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

### The Geometry of Virtuous Complexity: Nonlinear Pricing Kernels and the Limits of Linear Models

Linear asset pricing models do not merely underperform nonlinear ones — they impose a false geometry on the stochastic discount factor. Constructed a 41‑factor zoo spanning six model classes (OLS, Ridge, Lasso, ElasticNet, LightGBM, MLP) and eight loss configurations on the Gu et al. (2020) panel (94 characteristics, 1957–2016) to show that nonlinearity changes the *span* of the SDF.

- LGB factors are >94% orthogonal to Ridge counterparts; the LGB tangency portfolio is 73% unexplained by the full linear span
- PC3 of the zoo — 66.2% nonlinear by loading share — is significantly priced (*t* = 2.75); the nonlinear premium (1.11%/month, *t* = 2.70) nearly doubles in high‑volatility regimes
- Three implicit priors shape SDF estimation: the loss function (which states get weight), the model architecture (which function class the kernel inhabits), and shrinkage (which directions survive)
- KNS uniform shrinkage is itself a linearity prior; block‑diagonal shrinkage that respects spectral heterogeneity nearly doubles the out‑of‑sample Sharpe ratio

*Working paper (2026)*

---

### Sustainable Finance: ESG, Climate Risk, and Asset Pricing

Readings and lecture for Empirical Corporate Finance on the emerging sustainable finance literature. Surveyed the theoretical foundations and empirical frontiers of how externalities, heterogeneous investor preferences, and regulatory frictions interact with asset prices.

- Covered the Starks (2023) "value vs values" framework: disentangling whether ESG affects returns through priced risk or non‑pecuniary investor demand
- Reviewed Pedersen (2025) on sustainable finance as implicit carbon pricing — how residual externalities enter expected returns as a discount‑rate wedge when carbon taxes fall short of the social cost of carbon
- Examined Giglio et al. (2025) on nature and biodiversity loss as economic state variables and a research agenda for financial economics

*Lecture (2026)*

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