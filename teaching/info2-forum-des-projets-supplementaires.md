---
layout: default
title: INFO2 — forum des projets supplémentaires
lang: fr
permalink: /teaching/info2-2017-2019/forum-des-projets-supplementaires/
---

# Forum des projets supplémentaires

[← Info2]({{ '/teaching/info2-2017-2019/' | relative_url }})

## Coquilles

### Contenu de la cellule d'une liste

> Dans le sujet, vous indiquez que chaque cellule doit contenir 3 cases de mémoire. Pourtant, dans les transparents de cours, je vois que chaque case ne contient que deux arguments : sa valeur et l'adresse du nœud suivant. Quelle est la troisième case que j'ai ratée ?

Il y a une coquille dans le sujet :

- soit la liste utilisée par l'implémentation est *simplement* chaînée et deux cases suffisent,
- soit la liste utilisée par l'implémentation est *doublement* chaînée (chaînée dans les deux sens) et il faut trois cases mémoire.

Il me semble que la liste circulaire simplement chaînée des transparents de cours est suffisante, mais je vous laisse vérifier et choisir l'implémentation qui vous convient.

## Quelles informations doivent être stockées dans une mémoire réservée ?

> La question est dans le titre.

L'objectif pédagogique est de vous faire manipuler la réservation / libération de mémoire. Je ne vous demande donc pas de « réserver » toute la mémoire nécessaire à l'instanciation d'un objet, mais uniquement la partie de cette mémoire qui sert à stocker les valeurs contenues dans le vecteur.

Concrètement :

- pour les vecteurs s'appuyant sur une unique mémoire (de taille variable), seules les valeurs contenues dans le vecteur sont à stocker dans une mémoire « réservée » ;
- pour les vecteurs s'appuyant sur une liste chaînée, les cellules de la liste sont à instancier avec une mémoire « réservée » de taille 2 ou 3.

Les autres informations peuvent être stockées directement dans l'objet, sans tenir compte de la place mémoire qu'elles prennent. C'est le cas notamment de :

- la date de création du vecteur,
- la taille de la mémoire réservée,
- l'âge de l'utilisateur du vecteur,
- la référence vers la première case mémoire,
- le nombre de valeurs stockées dans le vecteur,
- la coiffure du capitaine,
- ...
