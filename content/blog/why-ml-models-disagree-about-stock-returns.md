---
title: "Why ML Models Disagree About Stock Returns"
date: 2026-04-06
draft: false
tags: ["machine-learning", "asset-pricing", "research"]
description: "When neural networks and gradient boosting look at the same stocks, they see different things. Here's why that disagreement is geometrically structured — and what it means for building better ensembles."
summary: "Model disagreement in asset pricing isn't noise — it's geometry. A look at what happens when you point different ML architectures at the same return prediction problem."
ShowToc: false
ShowReadingTime: true
---

When you train a neural network and a gradient boosting model on the same stock return data, they don't just give you different numbers — they disagree in *structured* ways. The neural network picks up on nonlinear interactions between firm characteristics. The boosted tree finds threshold effects and feature interactions that linear models miss entirely. And the regularized linear model? It sees a cleaner, lower-dimensional version of the same data.

This isn't a bug. It's information.

---

### The setup

In my current research, I train models from six different classes — ridge regression, elastic net, random forests, XGBoost, LightGBM, and neural networks — on the same panel of US stock returns spanning 1957-2024. Each model produces a set of "factors" (managed portfolios formed from its predictions). When you stack these factors together into a zoo and look at their covariance structure, something surprising happens.

The eigenvalue spectrum is *bimodal*. The linear models produce high-variance factors that cluster together. The nonlinear models produce lower-variance factors that are nearly orthogonal to the linear ones — subspace angles exceeding 70 degrees.

I call this **spectral segregation**.

---

### Why it matters

Most ensemble methods treat model disagreement as noise to be averaged away. But if the disagreement is geometrically structured — if different model classes are literally pointing in different directions in return space — then blind averaging destroys information.

The key insight: a model's deviation from the ensemble mean is only valuable if it aligns with the **stochastic discount factor** (the pricing kernel that tells you which directions in return space are compensated with risk premia). The cosine of the angle between a model's deviation vector and the SDF explains 64% of cross-model variation in deviation quality.

---

### The practical upshot

Instead of equal-weighting your ensemble or using generic stacking, you can weight models by how well their unique signals align with the pricing kernel. In out-of-sample tests, SDF-aligned ensembles roughly double the Sharpe ratio compared to uniform shrinkage.

The deeper lesson: model disagreement isn't just statistical variance. It reflects genuine differences in how architectures decompose the data-generating process. Understanding the geometry of that disagreement turns a liability into an edge.

---

*This post summarizes ideas from my working paper, "Which Directions Pay? A Geometric Theory of Model Disagreement in Asset Pricing." The full paper is in progress.*
