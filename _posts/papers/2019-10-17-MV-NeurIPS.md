---
layout: post
title: "High-Dimensional Multivariate Forecasting withLow-Rank Gaussian Copula Processes."
description: ""
category: "pub"
tags: [deep learning, forecasting]
status: 'Accepted: NeurIPS, 2019'
coauthor: David Salinas, Michael Bohlke-Schneider, Laurent Callot, Roberto Medico, Jan Gasthaus 
---




Download the [paper](https://arxiv.org/pdf/1910.03002.pdf).


## Abstract:

Predicting  the  dependencies  between  observations  from  multiple  time  series  iscritical  for  applications  such  as  anomaly  detection,  financial  risk  management,causal analysis, or demand forecasting. However, the computational and numeri-cal difficulties of estimating time-varying and high-dimensional covariance matri-ces often limits existing methods to handling at most a few hundred dimensions orrequires making strong assumptions on the dependence between series.  We pro-pose to combine an RNN-based time series model with a Gaussian copula processoutput model with a low-rank covariance structure to reduce the computationalcomplexity and handle non-Gaussian marginal distributions. This permits to dras-tically reduce the number of parameters and consequently allows the modeling oftime-varying correlations of thousands of time series.  We show on several real-world datasets that our method provides significant accuracy improvements overstate-of-the-art baselines and perform an ablation study analyzing the contribu-tions of the different components of our model.