---
layout: default
title: INFO2 — forum du projet
lang: fr
permalink: /teaching/info2-2017-2019/forum-du-projet/
---

# Forum du projet

[← Info2]({{ '/teaching/info2-2017-2019/' | relative_url }})

Je reporte sur cette page les questions qui m'ont été posées concernant ce projet et les réponses que j'ai fournies.

## Coquilles

### get_shape() vs. dimensions()

Dans la documentation de la fonction `get_shape()` de la classe `QTMatrix`, `m.dimensions()` est à remplacer par `m.get_shape()`.

### Oubli dans QTMatrix

Dans la documentation de la classe `QTMatrix`, il manque `>>>m1` entre `>>>m1[2,0]=3` et

```
[[4,0,0,0],
 [0,0,0,0],
 [3,-4,0,0]
 [0,0,0,0]]
```

### \_\_repr\_\_() retourne une chaîne de caractères

Dans la documentation de la fonction `__repr__()` de la classe `QTMatrix`, les tests devraient retourner des chaînes de caractères, et non pas les afficher. Donc

```
'[[2, 0, 0, 0],
 [0, 0, 0, 0],
 [0, -4, 0, 0],
 [0, 0, 0, 0]]'
```

est à remplacer par

```
'[[2, 0, 0, 0],\n [0, 0, 0, 0],\n [0, -4, 0, 0],\n [0, 0, 0, 0]]'
```

dans les deux cas : `str(QTMatrix(4, [0,2], [0,1], [2,-4]))` et `str(QTMatrix(4, [0,2], [0,1], [2,-4]))`.

## QTMatrix : une matrice ou un arbre ?

> Dans le fichier qtmatrix, j’ai quelques doutes au sujet des types des objets utilisés.
>
> J’ai pensé tout d’abord qu’il s’agit de simples listes de tableaux, comme le laisse suggérer le résultat attendu pour `__repr__` (dans l’exemple que vous avez mis en tête) :
>
> ```
> >>> QTMatrix(4, [0,2], [0,1], [2,-4])
>         [[2, 0, 0, 0],
>          [0, 0, 0, 0],
>          [0, -4, 0, 0],
>          [0, 0, 0, 0]]
> ```
>
> Un array numpy se représenterait en effet plutôt sous la forme (sans les virgules) :
>
> ```
> [[0 0 0 0]
> [0 0 0 0]
> [0 0 0 0]
> [0 0 0 0]]
> ```
>
> En revanche la fonction `__setitem__` renvoie une erreur qui me semble plus spécifique au type array de numpy (je ne l’ai jusqu’ici jamais rencontrée avec des listes…) :
>
> ```
> IndexError: index 4 is out of bounds for axis 0 with size 4
> ```
>
> Pourriez-vous donner une indication au sujet des types employés dans le fichier qtmatrix ?

```
[[2, 0, 0, 0],
 [0, 0, 0, 0],
 [0, -4, 0, 0],
 [0, 0, 0, 0]]
```

n'est qu'un affichage, il ne présume en rien de l'implémentation de la matrice. Techniquement, `__repr__()` retourne la chaîne de caractères `"[[2, 0, 0, 0],\n [0, 0, 0, 0],\n [0, -4, 0, 0],\n [0, 0, 0, 0]]"`, et l'interpréteur Python affiche cette chaîne de caractères.

Il en va de même pour `__setitem__(self)` : le message d'erreur porte sur le concept de matrice, il est indépendant du stockage en interne des valeurs de la matrice.

Il faut bien faire la distinction entre l'interface (ie. les fonctionnalités fournies à l'utilisateur) et l'implémentation de cette interface. À titre d'illustration, il me semble que cette même interface est aussi utilisée pour les classes `numpy.array` (tenseurs), `numpy.matrix`, et `scipy.sparse.spmatrix` (matrices creuses) ; et pourtant ces trois classes manipulent des données bien différentes en interne.

Dans le cadre de ce projet, en interne les données doivent être stockées dans un QuadTree. Même si l'utilisateur de la classe `QTMatrix` doit avoir l'impression de manipuler une matrice.

## Construction récursive de la QTMatrix

> Je me trouve un peu bloqué sur le td au moment de définir `__init__` pour les QTMatrices. J'étais au départ parti dans l'idée de créer deux attributs, 1) la taille et 2) l'arbre associé à la matrice mais je n'arrive pas à créer de manière récursive cet arbre.
>
> Je me suis donc dit qu'il fallait juste définir les QTMatrices comme 1) une taille et 2) si `vals==None` ou si `vals==[]` : une valeur / sinon : les 4 matrices formant les carrés de la matrice principale. Cette méthode repousse donc l'usage des arbres au moment de `__repr__`.
>
> Ma question est donc : pouvons-nous créer un `__init__` de manière récursive ? Sinon, la deuxième méthode employée est-elle moralement mauvaise ?

Une QTMatrix est une boîte, qui contient un arbre. Cet arbre est un objet par nature récursif, et se manipule donc très bien de façon récursive ; la boîte non. En d'autres termes, la fonction `__init__()` a peu de chance d'être récursive, mais elle peut faire appel à une fonction récursive pour travailler sur l'arbre contenu dans l'objet QTMatrix.

La solution la plus jolie serait par exemple d'avoir dans `__init__()` une opération de la forme `self.qt = build_qt_rec(inds_i, inds_j, vals)`, où `build_qt_rec()` serait une fonction récursive retournant le QuadTree approprié.

Une solution un peu moins jolie, mais quasiment aussi efficace serait de commencer par définir un arbre correspondant à la matrice vide, puis remplir cet arbre en ajoutant les valeurs une par une.

## Quelles fonctions décorer ?

> Est-ce qu'il faut documenter les fonctions auxiliaires à l'intérieur des définitions des méthodes ?

Je désire simplement une preuve du fait que vous savez commenter une fonction en incluant des tests unitaires. Il suffit donc de compléter les commentaires des fonctions pré-existantes du fichier `quadtree.py` :

- `copy()`
- `__repr__()`
- `is_a_leaf()`
- `is_internal()`
- `get_val()`
- `set_val()`
- `get_son()`
- `set_son()`
- `internal_node()`
- `leaf()`

## Simplification de l'arbre

> Si on a la matrice `m = [ [0,0], [0,1] ]` et qu'on exécute `m[1,1] = 0`, attendez-vous de nous que m soit
>
> ```
>  |
>  0
> ```
>
> ou
>
> ```
>  /  |  |  \
> 0   0  0   0
> ```
>
> En clair, faut-il « simplifier » les matrices quand elles se creusent ?

Ce n'est pas demandé, mais j'ajouterai des points de bonus si c'est fait.
