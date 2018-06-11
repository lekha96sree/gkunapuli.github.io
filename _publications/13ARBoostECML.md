---
title: "AR-Boost: Reducing Overfitting by a Robust Data-Driven Regularization Strategy"
collection: publications
permalink: /publication/13ARBoostECML
excerpt: ''
date: 2013-09-01
venue: 'Twenty-Fourth European Conference on Machine Learning (ECML''13), Prague, Czech Republic'
paperurl: 'http://gkunapuli.github.io/files/13ARBoostECML.pdf'
citation: 'B. Saha, G. Kunapuli, N. Ray, J. Maldjian and S. Natarajan. <b> AR-Boost: Reducing Overfitting by a Robust Data-Driven Regularization Strategy </b>. <i> Twenty-Fourth European Conference on Machine Learning </i> (ECML''13), Prague, Czech Republic, September 23-27, 2012.'
---

We introduce a novel, robust data-driven regularization strategy called Adaptive Regularized Boosting (AR-Boost), motivated by a desire to reduce overfitting. We replace AdaBoost's hard margin with a regularized soft margin that trades-off between a larger margin, at the expense of misclassification errors. Minimizing this regularized exponential loss results in a boosting algorithm that relaxes the weak learning assumption further: it can use classifiers with error greater than 1 2 . This enables a natural extension to multiclass boosting, and further reduces overfitting in both the binary and multiclass cases. We derive bounds for training and generalization errors, and relate them to AdaBoost. Finally, we show empirical results on benchmark data that establish the robustness of our approach and improved performance overall.

[[BibTeX]](http://gkunapuli.github.io/files/13ARBoostECML.bib)
