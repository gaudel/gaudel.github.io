---
layout: default
title: ADM 2025
permalink: /teaching/adm-2025/
---

# ADM — Analyse de Données et Modélisation probabiliste

**M. Sc. course — Data analysis and probabilistic modeling**

*Making data speak: Advanced probabilistic data analysis and modeling*

> **Disclaimer:** Courses mainly based on [Guillaume Gravier's original course](http://people.irisa.fr/Guillaume.Gravier/ADM/). I thank a lot Guillaume for the course material and for his numerous recommendations regarding the details of the course.

Data, whatever they are, are of very limited value without the possibility to extract valuable information to better synthesize, understand, predict. Statistical methods for data analysis and probabilistic models for statistical machine learning are commonly used to do so. This course aims at acquiring the basic techniques for data analysis (exploratory statistics) and probabilistic modeling (inferential statistics) and to study their application to different types of data (symbolic data, language, numerical data, signals, images, etc.). The lectures naturally articulate around the two major steps of any modeling process: understand your data then design an adequate model.

**Keywords:** data analysis, factor analysis, variance analysis, clustering, hypothesis testing, decision theory, estimation theory, Gaussian mixture models, EM algorithm, Markov chains, Markov fields, hidden Markov chains, Viterbi algorithm, Bayesian networks, token passing algorithm

## Lectures, with the 2025-2026 dates

*(Lectures are 1.5-hour sessions, held in Room Guernesey unless otherwise specified)*  
*(\[prev.\] indicates last year material which may be updated during the semester)*

- **Wed. Sep. 10, 8h.** [A gentle reminder of the basics of probability: Kolmogorov](https://drive.google.com/file/d/1GaEdd3fHiTHVgfdIdWyNY9NmRszHGn6e/view?usp=sharing)
- **Fri. Sep. 12, 8h.** [A gentle reminder of the basics of probability: random variables, moments, classical laws](https://drive.google.com/file/d/1GaEdd3fHiTHVgfdIdWyNY9NmRszHGn6e/view?usp=sharing)
- **Wed. Sep. 17, 8h.** [Exploratory statistics: visualization, summaries, correlation](https://drive.google.com/file/d/1YS6Ogdkz5Sm6PsuMNsaNGfVrj8_K72F_/view?usp=sharing)
- **Fri. Sep. 19, 8h.**
  - [Exploratory statistics: PCA/LDA](https://drive.google.com/file/d/1YS6Ogdkz5Sm6PsuMNsaNGfVrj8_K72F_/view?usp=sharing)
  - [Cluster analysis: k-means](https://drive.google.com/file/d/14ZNPcmZfMxm0dTRx9LgAslqFkeOCv7If/view?usp=sharing)
- **Thu. Sep. 25, 8h.**
  - [Cluster analysis: agglomerative/divisive clustering, spectral clustering and other weird things](https://drive.google.com/file/d/14ZNPcmZfMxm0dTRx9LgAslqFkeOCv7If/view?usp=sharing)
- **Fri. Sep. 26, 8h.** [Fundamentals of statistical machine learning and estimation theory: cost function, decision theory, basic estimators](https://drive.google.com/file/d/14p2Gk68fPIt8p-1J9grndLEwPrK7_zCH/view?usp=sharing)
- **Wed. Oct. 1, 8h.** [Fundamentals of statistical machine learning and estimation theory: estimation theory, practical estimation techniques](https://drive.google.com/file/d/14p2Gk68fPIt8p-1J9grndLEwPrK7_zCH/view?usp=sharing)
- **Wed. Oct. 8, 8h.** [Mixture models: mixture models, hidden variables, estimation-maximization (EM) algorithm](https://drive.google.com/file/d/1DccEdGjikjHYwC1wyzSQ730Ki8EWgM07/view?usp=sharing)
  - see also [handnotes on the EM for a two Gaussian mixture model](http://people.irisa.fr/Guillaume.Gravier/ADM/two-gaussians-EM-notes.pdf)
- **Fri. Oct. 10, 8h.** [Observable and hidden Markov models: Markov property, Markov chain, hidden Markov chain, Viterbi algorithm, Baum-Welsh algorithm, practical examples](https://drive.google.com/file/d/11PQDJr23Yo5A3qPVw95Sv79QV97hbouk/view?usp=sharing)
- **Wed. Oct. 15, 8h.** [Observable and hidden Markov models: Markov property, Markov chain, hidden Markov chain, Viterbi algorithm, Baum-Welsh algorithm, practical examples](https://drive.google.com/file/d/11PQDJr23Yo5A3qPVw95Sv79QV97hbouk/view?usp=sharing)
- **Wed. Oct. 22, 8h.** [Graphical models and Bayesian network: directed/undirected graphical models, Bayesian networks, inference and reasoning, moralization, variable elimination, junction tree algorithm](https://drive.google.com/file/d/1o7yL1h16Bfdoa-qWLRNkp-EAGId0OXHh/view?usp=drive_link)
- **Thu. Oct. 23, 8h.** [Entropy and conditional random fields: maximum entropy principle, maxent model, logistic regression, log-linear sequence models, parameter estimation](https://drive.google.com/file/d/10wgxJCrLukIfJGF1W8a63ldZ8n7zlsCt/view?usp=drive_link)
- **Wed. Nov. 5, 8h.** [Hypothesis testing: typology, likelihood ratio test, classical mean value tests, comparison and statistical significance, variance analysis](https://drive.google.com/file/d/16jmfH1MXLjpp8L7wb1TXFebF52ELcTj4/view?usp=sharing)
- **Wed. Nov. 12, 8h.** [Hypothesis testing: multiple-hypothesis testing, exercices](https://drive.google.com/file/d/16jmfH1MXLjpp8L7wb1TXFebF52ELcTj4/view?usp=sharing)
- **Wed. Nov. 19, 8h.** Final exam.

## Evaluation / exams

- **Homework.** Write a short comment on either one of the articles below. Maximum length is 1000 words, ca. 1.5-2 pages single column 11 point font (English or French, as you wish). Your report shall identify the techniques seen in the classroom, explain why they are appropriate in the context of this paper and what efforts authors have made to cast their work into a probabilistic framework, explain how they were adapted and/or extended, discuss the limits you foresee (whether mentioned in the paper or not). Deadline for mailing comment: before Nov. 12, 2024, 08:00 CET
  - Douglas Reynolds, Thomas Quatieri and Robert Dun. [Speaker verification using adapted Gaussian mixture models](http://people.irisa.fr/Guillaume.Gravier/ADM/articles2020/reynolds-00.pdf). Digital Signal Processing, 10:19-41, 2000
  - Laurens van der Maaten and Geoffrey Hinton. [Visualizing data using t-SNE](http://people.irisa.fr/Guillaume.Gravier/ADM/articles2020/vandermaaten-08.pdf). Journal of Machine Learning Research, 9:2579-2605, 2008
  - Tao Xiang and Shaogang Gong. [Spectral clustering with eigen vector selection](http://people.irisa.fr/Guillaume.Gravier/ADM/articles2020/xiang-08.pdf). Pattern recognition letter, 41:1012-1029, 2008
- **Final exam.** Standard 1h30 written exam. You can check the text of past exams below.
  - 2023: [in French](https://drive.google.com/file/d/1GpwPGJmiMTJ3b2-2WXmnp-iFlNHLMvuh/view?usp=sharing), [in English](https://drive.google.com/file/d/10WQfcBdk_gMOZYISuKRuZfzmcpGMfyeK/view?usp=sharing)
  - 2022: [in French](https://drive.google.com/file/d/1KFNpyZ7nfWzEpQ2hWYT62IMg9hn4-FjY/view?usp=sharing), [in English](https://drive.google.com/file/d/1wNa1gJrJlAL4nANJ1aIqKqg3O-G7Fh66/view?usp=sharing)
  - 2019: [in French](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-19-fr.pdf)
  - 2018: [in French](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-18-fr.pdf), [in English](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-18-en.pdf)
  - 2017: [in French](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-17-fr.pdf), [in English](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-17-en.pdf)
