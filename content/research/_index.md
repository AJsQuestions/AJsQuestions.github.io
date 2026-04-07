---
title: "Research"
aliases: /research
description: "Papers and projects"
tags: ["asset-pricing", "machine-learning", "financial-econometrics"]
---

### Interests

- Empirical Asset Pricing
- Machine Learning
- High-Dimensional Econometrics
- Financial Data Science

---

### Which Directions Pay? A Geometric Theory of Model Disagreement in Asset Pricing

When ML models disagree about stock returns, alignment with the stochastic discount factor predicts which deviations carry useful information. The cosine of the angle between a model's deviation vector and the SDF explains 64% of cross-model variation in deviation quality — suggesting that model disagreement is geometrically structured, not noise.

- Built on the Gu et al. (2020) / JKP panel spanning 1957-2024 with WRDS/CRSP/Compustat data
- Trained neural networks, gradient boosting (XGBoost, LightGBM, CatBoost), and regularized linear models on UCLA's Hoffman2 GPU cluster
- SDF-aligned ensembles improve out-of-sample Sharpe ratios relative to equal-weight and stacking baselines
- Connects to the spectral segregation finding: nonlinear models contribute orthogonal directions that uniform shrinkage kills

*Working paper (2026) — actively developing*

---

### The Geometry of Virtuous Complexity: Spectral Segregation, Shrinkage, and the Pricing Kernel

When a factor zoo mixes linear and nonlinear models, the covariance matrix develops a bimodal eigenvalue spectrum — *spectral segregation*. Uniform ridge shrinkage calibrated to the joint zoo preserves high-variance linear directions and kills lower-variance nonlinear ones, acting as an implicit linearity prior.

- A 41-factor zoo spanning six model classes and eight loss configurations on the Gu et al. (2020) panel (1957-2016) verifies every prediction of the theory
- LGB factors are >94% orthogonal to Ridge counterparts (subspace angle 71.3°); the nonlinear premium (1.54%/month, NW *t* = 4.89) reflects convex market exposure and survives eight-factor controls
- Block-diagonal shrinkage doubles the out-of-sample Sharpe ratio (0.24 vs 0.12); five-fold cross-validated HJ distances confirm the result

*Working paper (2026)*

---

### Sustainable Finance: ESG, Climate Risk, and Asset Pricing

Surveyed the theoretical foundations and empirical frontiers of how externalities, heterogeneous investor preferences, and regulatory frictions interact with asset prices.

- Starks (2023): disentangling whether ESG affects returns through priced risk or non-pecuniary demand
- Pedersen (2025): sustainable finance as implicit carbon pricing — residual externalities as a discount-rate wedge
- Giglio et al. (2025): biodiversity loss as economic state variables

*Lecture (2026)*

---

### Automating Black-Litterman Beliefs with Machine Learning

Replacing subjective investor views in Black-Litterman Portfolio Optimization with structured ML-generated beliefs. Links Bayesian portfolio theory with prediction without discarding economic intuition.

*Working paper (2024)*

---

### Illiquidity & Expected Returns

Harvard Business School, with Profs. Victoria Ivashina and Josh Lerner. Analyzed how illiquidity, smoothing, and valuation practices affect measured expected returns using Mean-Variance and Black-Litterman frameworks across alternative asset classes.

---

### Return Attribution & Causality

Harvard Business School, with Profs. Victoria Ivashina and Josh Lerner. Conducted return decompositions and applied synthetic control methods using large-scale firm-level panel data.

---

### Empirical Asset Pricing & ML

Booth School of Business, with Prof. Dacheng Xiu. Applied regularized and nonlinear ML methods to study pricing errors and latent factor structure in housing and consumer credit markets, separating systematic risk from idiosyncratic noise.

---

### High-Dimensional Credit Models

Booth School of Business, with Prof. Dacheng Xiu. Built default prediction models using borrower- and loan-level characteristics; assessed stability, shrinkage behavior, and economic interpretability across specifications.

---

### Ensemble Machine Learning

Indian Statistical Institute, with Prof. Tanujit Chakraborty. Focused study of ensemble and hybrid ML methods, emphasizing bias-variance tradeoffs.

---

### Real Estate Pricing and Presale Option Risk

IIM Bangalore, with Prof. Venkatesh Panchapagesan. Developed pricing models for presale real estate markets, estimating risk premia linked to project-level uncertainty and market cycles.
