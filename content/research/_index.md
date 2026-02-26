---
title: "Research"
aliases: /research
description: "Papers and projects"
---

### Interests

- Empirical Asset Pricing
- Mathematical and Computational Finance
- Financial Econometrics and Statistics
- Machine Learning and Data Science

---

### Loss as Prior: Training Objectives and Pricing‑Kernel Geometry

The training loss in ML asset pricing is not a nuisance parameter — it is an implicit economic prior over which states of the world matter for constructing the pricing kernel. I construct a 41‑factor zoo spanning four model classes (Dense, Sparse, LightGBM, MLP) and eight loss configurations, using the Gu et al. (2020) panel of 94 characteristics and monthly returns (1957–2016).

- Economic‑loss factors (Sharpe, Soft, Spread) dominate MSE within every architecture, with gains increasing in model flexibility: MLP +124%, LGB +24%, Ridge +3%
- The 41‑factor zoo has 13 statistically significant principal components and jointly rejects FF6 spanning (GRS = 1,044, *p* < 0.001); all LGB factors deliver monthly alphas exceeding 1.4%
- Nonlinear models learn genuinely different pricing directions — LGB factors are >94% orthogonal to their Ridge counterparts across all eight losses
- KNS shrinkage concentrates the zoo from 17 to 1.4 effective dimensions; 24 of 41 factors survive the double‑LASSO pricing test

*Working paper (2026)*

---

### Automating Black–Litterman Beliefs with Machine Learning

Replacing subjective investor views in Black–Litterman Portfolio Optimization with structured ML‑generated beliefs.

- Links Bayesian portfolio theory with prediction without discarding economic intuition
- Keeps the model transparent so you can see when the data is steering the ship
- Early results show portfolios that beat naïve baselines without hiding risk

*Working paper (2024)*

---

### Illiquidity, Volatility Smoothing, and Portfolio Risk

Research at Harvard Business School with Profs Victoria Ivashina and Josh Lerner. Mean–variance and Black–Litterman simulations to estimate the fixed cost of illiquidity on risk premiums of alternative asset classes like private equity and real estate, in contrast with fixed income and public equity.

---

### Killer Acquisitions and Innovation in FinTech

Research at Harvard Business School with Profs Victoria Ivashina and Josh Lerner. Synthetic control regressions to test the causal effect of M&A on innovation throughput for FinTech firms.

---

### ML for Empirical Asset Pricing

Research at Chicago Booth with Prof Dacheng Xiu. Applied machine learning to empirical pricing problems including real estate valuation (Zillow Zestimate) and credit default prediction (LendingClub).

---

### Ensemble Machine Learning for Time Series

Summer research at the Indian Statistical Institute with Prof Tanujit Chakraborty. Readings and experiments in ensemble and hybridized machine learning models for time series analysis.

---

### Real Estate Pricing and Presale Option Risk

Research at IIM Bangalore with Prof Venkatesh Panchapagesan. Structural models of presale housing markets, quantifying risk premia and how information asymmetry shapes urban real estate.