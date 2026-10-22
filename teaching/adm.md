---
layout: default
title: ADM
permalink: /teaching/adm/
---

# ADM — Analyse de Données et Modélisation probabiliste

**M. Sc. course — Data analysis and probabilistic modeling**

*Making data speak: Advanced probabilistic data analysis and modeling*

> **Disclaimer:** Courses mainly based on [Guillaume Gravier's original course](http://people.irisa.fr/Guillaume.Gravier/ADM/). I thank a lot Guillaume for the course material and for his numerous recommendations regarding the details of the course.

Data, whatever they are, are of very limited value without the possibility to extract valuable information to better synthesize, understand, predict. Statistical methods for data analysis and probabilistic models for statistical machine learning are commonly used to do so. This course aims at acquiring the basic techniques for data analysis (exploratory statistics) and probabilistic modeling (inferential statistics) and to study their application to different types of data (symbolic data, language, numerical data, signals, images, etc.). The lectures naturally articulate around the two major steps of any modeling process: understand your data then design an adequate model.

**Keywords:** data analysis, factor analysis, variance analysis, clustering, hypothesis testing, decision theory, estimation theory, Gaussian mixture models, EM algorithm, Markov chains, Markov fields, hidden Markov chains, Viterbi algorithm, Bayesian networks, token passing algorithm

## Lectures, with the 2026-2027 dates

*(Lectures are 1.5-hour sessions, held in Room Guernesey unless otherwise specified)*  
*(\[prev.\] indicates last year material which may be updated during the semester)*

- **Wed. Sep. 9, 8h.** [A gentle reminder of the basics of probability]({{ '/files/adm-1.pdf' | relative_url }}) : Kolmogorov
- **Fri. Sep. 11, 8h.** [A gentle reminder of the basics of probability]({{ '/files/adm-1.pdf' | relative_url }}): random variables, moments, classical laws
- **Wed. Sep. 17, 9h45.** [Exploratory statistics]({{ '/files/adm-2.pdf' | relative_url }}): visualization, summaries, correlation
- **Fri. Sep. 18, 8h.**
  - [Exploratory statistics]({{ '/files/adm-2.pdf' | relative_url }}): PCA/LDA
  - [Cluster analysis]({{ '/files/adm-3.pdf' | relative_url }}): k-means
- **Mon. Sep. 21, 8h.**
  - [Cluster analysis]({{ '/files/adm-3.pdf' | relative_url }}): agglomerative/divisive clustering, spectral clustering and other weird things
- **Tue. Sep. 22, 16h45.** [Fundamentals of statistical machine learning and estimation theory]({{ '/files/adm-4.pdf' | relative_url }}): cost function, decision theory, basic estimators
- **Tue. Sep. 29, 16h45.** [Fundamentals of statistical machine learning and estimation theory]({{ '/files/adm-4.pdf' | relative_url }}): estimation theory, practical estimation techniques
- **Wed. Sep. 30, 8h.** [Mixture models]({{ '/files/adm-5.pdf' | relative_url }}): mixture models, hidden variables, estimation-maximization (EM) algorithm
  - see also [handnotes on the EM for a two Gaussian mixture model](http://people.irisa.fr/Guillaume.Gravier/ADM/two-gaussians-EM-notes.pdf)
- **Tue. Oct. 6, 17h45.** [Observable and hidden Markov models]({{ '/files/adm-6.pdf' | relative_url }}): Markov property, Markov chain, hidden Markov chain
- **Tue. Oct. 13, 13h15.** [Observable and hidden Markov models]({{ '/files/adm-6.pdf' | relative_url }}): Viterbi algorithm, Baum-Welsh algorithm, practical examples
- **Wed. Oct. 14, 11h30.** [Graphical models and Bayesian network]({{ '/files/adm-7.pdf' | relative_url }}): directed/undirected graphical models, Bayesian networks, inference and reasoning, moralization, variable elimination, junction tree algorithm
- **Thu. Oct. 15, 9h45.** [Entropy and conditional random fields]({{ '/files/adm-8.pdf' | relative_url }}): maximum entropy principle, maxent model, logistic regression, log-linear sequence models, parameter estimation
- **Tue. Oct. 20, 13h15.** [Hypothesis testing]({{ '/files/adm-9.pdf' | relative_url }}): typology, likelihood ratio test, classical mean value tests, comparison and statistical significance, variance analysis
- **Fri. Oct. 23, 11h30.** Exercices
- **Tue. Nov. 3, 13h15.** Final exam

## Evaluation / exams

- **Homework.** Write a short comment on either one of the articles below. Maximum length is 1000 words, ca. 1.5-2 pages single column 11 point font (English or French, as you wish). Your report shall identify the techniques seen in the classroom, explain why they are appropriate in the context of this paper and what efforts authors have made to cast their work into a probabilistic framework, explain how they were adapted and/or extended, discuss the limits you foresee (whether mentioned in the paper or not). Deadline for mailing comment: **before Nov. 10, 2026, 08:00 CET**
  - Douglas Reynolds, Thomas Quatieri and Robert Dun. [Speaker verification using adapted Gaussian mixture models]({{ '/files/reynolds-00.pdf' | relative_url }}). Digital Signal Processing, 10:19-41, 2000
  - Laurens van der Maaten and Geoffrey Hinton. [Visualizing data using t-SNE]({{ '/files/vandermaaten-08.pdf' | relative_url }}). Journal of Machine Learning Research, 9:2579-2605, 2008
  - Tao Xiang and Shaogang Gong. [Spectral clustering with eigen vector selection]({{ '/files/xiang-08.pdf' | relative_url }}). Pattern recognition letter, 41:1012-1029, 2008
- **Final exam.** Standard 1h30 written exam. You can check the text of past exams below.
  - 2025: [in French]({{ '/files/exam-nov-25-fr.pdf' | relative_url }})
  - 2024: [in French]({{ '/files/exam-nov-24-fr.pdf' | relative_url }}), [in English]({{ '/files/exam-nov-24-en.pdf' | relative_url }})
  - 2023: [in French]({{ '/files/exam-nov-23-fr.pdf' | relative_url }}), [in English]({{ '/files/exam-nov-23-en.pdf' | relative_url }})
  - 2022: [in French]({{ '/files/exam-nov-22-fr.pdf' | relative_url }}), [in English]({{ '/files/exam-nov-22-en.pdf' | relative_url }})
  - 2019: [in French](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-19-fr.pdf)
  - 2018: [in French](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-18-fr.pdf), [in English](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-18-en.pdf)
  - 2017: [in French](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-17-fr.pdf), [in English](http://people.irisa.fr/Guillaume.Gravier/ADM/exam-nov-17-en.pdf)
