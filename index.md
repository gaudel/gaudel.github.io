---
layout: default
title: Home
---

# Romaric Gaudel

{% assign photo = site.static_files | where: "path", "/assets/img/photo.jpg" | first %}
<div class="profile">
  {% if photo %}<img src="{{ '/assets/img/photo.jpg' | relative_url }}" alt="Photo of Romaric Gaudel">{% endif %}
  <div class="info" markdown="1">
<p class="role">Assistant Professor (with "HdR")</p>

romaric.gaudel AT irisa.fr

**University:** [Univ. Rennes](https://www.univ-rennes.fr/)  
**Lab / institute:** [IRISA](https://www.irisa.fr/en) / [Inria](https://www.inria.fr/fr/centre-inria-universite-rennes) (Rennes)  
**Team:** [MALT](https://team.inria.fr/malt/)
  </div>
</div>

Since 2022, I'm Assistant Professor (Maître de Conférences) at [Univ. Rennes](https://www.univ-rennes.fr/) and I'm carrying my research at [IRISA](https://www.irisa.fr/en) laboratory in the newly founded [MALT](https://team.inria.fr/malt/) [Inria](https://www.inria.fr/en/centre/rennes) project-team. I'm mostly enjoying playing with [bandits](https://en.wikipedia.org/wiki/Multi-armed_bandit) and [Recommender Systems](https://en.wikipedia.org/wiki/Recommender_system), and with Machine Learning in general, including Interpretable Machine Learning and approaches preserving the privacy.

In the past:

- I obtained a Master Research degree in Computer Science in 2006 after 3 years of study at [brittany part of ENS Cachan](http://www.bretagne.ens-cachan.fr/).
- I was PhD student from 2006 to 2010 at [Univ. Paris-Sud](http://www.u-psud.fr/) (France). I was member of the Machine Learning / Optimization team ([A&O-TAO](http://tao.lri.fr/)) in [LRI](http://www.lri.fr/) (UMR [Univ. Paris-Sud](http://www.u-psud.fr/)/[CNRS](http://www.cnrs.fr/) n° 8623) under the supervision of [Michèle Sebag](http://www.lri.fr/~sebag) and [Antoine Cornuéjols](http://www.lri.fr/~antoine).
- From 2010 to 2011, I was PostDoc at [Télécom-ParisTech](http://www.telecom-paristech.fr/) (France) in collaboration with [Stéphan Clémençon](http://perso.telecom-paristech.fr/~clemenco/) in the team [STA](http://www.tsi.telecom-paristech.fr/sta/) (Statistics).
- From 2011 to 2017, I was Assistant Professor (Maître de Conférences) in the [Inria team SequeL](https://sequel.lille.inria.fr/) and member of [CRIStAL](http://www.cristal.univ-lille.fr/) (UMR [Lille1](http://www.univ-lille1.fr/)/[CNRS](http://www.cnrs.fr/) n° 9189) at University [Lille 3](http://www.univ-lille3.fr/).
- From 2017 to 2022, I was Assistant Professor at [ENSAI](http://ensai.fr/) and I was doing my research in the department of statistics of [CREST](http://www.crest.fr/) research center. In the meanwhile, I was external collaborator of [LACODAM](https://team.inria.fr/lacodam/) [Inria](https://www.inria.fr/en/centre/rennes) team at [IRISA](https://www.irisa.fr/en).

Take a look at my [resume]({{ '/resume/' | relative_url }}) for more details.

## Interests

### Current

- Machine Learning
- (online) Recommender Systems
- Bandit Theory
- Explanation of learned models
- Differential Privacy for Decentralized Learning

### Past (but still alive)

- (online) Matrix Completion
- Consensus ranking
- Feature Selection
- Multiple Instance Learning
- Phase Transition
- UCT (Upper Confidence bound Applied to Trees)
