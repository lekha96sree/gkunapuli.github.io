---
title: "Mirror Descent for Metric Learning: A Unified Approach"
collection: publications
permalink: /publication/12mdmlECML
excerpt: ''
date: 2012-09-01
venue: 'Twenty-Third European Conference on Machine Learning (ECML''12), Bristol, United Kingdom'
paperurl: 'http://gkunapuli.github.io/files/12mdmlECML.pdf'
citation: 'G. Kunapuli and J. W. Shavlik. <b> Mirror Descent for Metric Learning: A Unified Approach. </b> <i> Twenty-Third European Conference on Machine Learning </i> (ECML''12), Bristol, United Kingdom, September 24-29, 2012.'
author: '<b> G. Kunapuli </b> and J. W. Shavlik'
---

Most metric learning methods are characterized by diverse loss functions and projection methods, which naturally begs the question: is there a wider framework that can generalize many of these methods? In addition, ever persistent issues are those of scalability to large data sets and the question of kernelizability. We propose a unified approach to Mahalanobis metric learning: an online regularized metric learning algorithm based on the ideas of composite objective mirror descent (comid). The metric learning problem is formulated as a regularized positive semidefinite matrix learning problem, whose update rules can be derived using the comid framework. This approach aims to be scalable, kernelizable, and admissible to many different types of Bregman and loss functions, which allows for the tailoring of several different classes of algorithms. The most novel contribution is the use of the trace norm, which yields a sparse metric in its eigenspectrum, thus simultaneously performing feature selection along with metric learning.

[[BibTeX]](http://gkunapuli.github.io/files/12mdmlECML.bib)
[[Code]](https://github.com/gkunapuli/mdml)
