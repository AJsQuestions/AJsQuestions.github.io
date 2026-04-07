---
title: "What Regularization Actually Does to Your Portfolio"
date: 2026-03-20
draft: false
tags: ["asset-pricing", "machine-learning", "teaching"]
description: "Ridge regression doesn't just shrink coefficients — it encodes a belief about which directions in return space matter. Here's the geometric intuition."
summary: "Ridge regression doesn't just shrink coefficients — it encodes a prior about which directions in return space are worth betting on."
ShowToc: false
ShowReadingTime: true
---

When I TA'd Financial Econometrics at Booth, students would ask: *why does ridge regression improve out-of-sample performance?* The standard answer — "it reduces variance at the cost of some bias" — is correct but unsatisfying. It doesn't explain *what* ridge is actually doing to your portfolio.

Here's a more useful way to think about it.

---

### The portfolio view

Every linear regression on stock returns implicitly constructs a portfolio. The coefficients are weights. The predicted return is the portfolio's expected payoff. When you add a ridge penalty, you're not just shrinking numbers toward zero — you're rotating your portfolio toward the directions of highest variance in the data.

Ridge penalizes the *norm* of the coefficient vector. In the eigenspace of the covariance matrix, this means high-variance principal components get preserved while low-variance ones get killed. The shrinkage isn't uniform in economic terms — it's uniform in statistical terms, which has very non-uniform economic consequences.

---

### Why this matters for asset pricing

In asset pricing, the low-variance directions are often where the interesting signals live. Small anomalies, conditional patterns, nonlinear interactions — these show up in eigenvectors that ridge shrinkage aggressively dampens.

This is exactly the **spectral segregation** problem I study in my research. When you mix linear and nonlinear factors in a zoo, the nonlinear factors tend to have lower eigenvalues. Ridge shrinkage, calibrated on the full zoo, systematically kills these directions — even when they carry genuine risk premia.

The result: your "regularized" model isn't just simpler. It's encoding a very specific belief — that the high-variance, linear directions are the ones worth betting on. Sometimes that's right. Often it's not.

---

### The teaching takeaway

When I explain regularization in class, I start with geometry, not formulas. Draw the ellipse (the constraint set). Draw the contour lines (the loss surface). Show where they touch. Then ask: *what did we just assume about reality by choosing this shape?*

Every regularizer is a prior. The question is whether it's the prior you actually believe.
