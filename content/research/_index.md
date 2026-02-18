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

### When Does the Loss Function Matter? Model Class and Training Objective in ML Asset Pricing

Systematically estimating five model classes under six training objectives to ask a pointed question: when you build an ML pricing kernel, does the loss function change the answer, or does the function space you search over decide it for you?

- 25 model‑loss factors evaluated on 3.1 million firm‑month observations (1957–2016)
- PCA on the factor zoo reveals only 2–3 significant dimensions; factors cluster by model class, not objective
- Within‑class return correlations above 0.95 for linear models—Ridge absorbs all six losses without flinching
- LightGBM dominates economically (~1.75 annualized Sharpe) but diverges sharply under tail‑altering losses like MAE

The punchline: model class constrains the admissible set of SDF directions; the training objective just picks a point inside it. Research effort is better spent on function class design than objective engineering.

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