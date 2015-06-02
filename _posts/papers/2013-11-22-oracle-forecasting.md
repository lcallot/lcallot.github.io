---
layout: post
title: "Oracle Efficient estimation and Forecasting with the Adaptive Lasso and the Adaptive Group Lasso in Vector Autoregressions."
description: ""
category: "pub"
tags: [working paper, Forecasting, VAR, Lasso, High dimension]
status: 'Published in: Essays in Nonlinear Time Series Econometrics, Oxford University Press, 2014.'
coauthor: Anders Bredahl Kock
---

**Published as: Callot, Laurent A. F., and Anders Bredahl Kock, 2014, Oracle Efficient Estimation and Forecasting with the Adaptive Lasso and the Adaptive Group Lasso in Vector Autoregressions, in N. Haldrup, M. Meitz, and P. Saikkonen (eds.), Essays in Nonlinear Time Series Econometrics, Oxford University Press.**

Download the paper [pdf]({{ site.url }}/papers/oracle_forecast.pdf).

[Replication material](https://github.com/lcallot/lasso-macro-forecast).

## Abstract:
We show that the adaptive Lasso (aLasso) and the adaptive group Lasso (agLasso) are oracle efficient in stationary vector autoregressions where the number of parameters per equation is smaller than the number of observations. In particular, this means that the parameters are estimated consistently at a √T -rate, that the truly zero parameters are classified as such asymptotically and that the non-zero parameters are estimated as efficiently as if only the relevant variables had been included in the model from the outset. The group adaptive Lasso differs from the adaptive Lasso by dividing the covariates into groups whose members are all relevant or all irrelevant. Both estimators have the property that they perform variable selection and estimation in one step. We evaluate the forecasting accuracy of these estimators for a large set of macroeconomic variables. The plain Lasso is found to be the most precise procedure overall. The adaptive and the adaptive group Lasso are less stable but mostly perform at par with common factor models.
