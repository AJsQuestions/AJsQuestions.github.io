---
title: "What I Learned Building a Football Prediction System"
date: 2026-02-15
draft: false
tags: ["machine-learning", "data-science", "projects"]
description: "FootieM8 covers 25+ leagues across 30 seasons. The models work. The markets are harder."
summary: "Building a research-grade match prediction system taught me more about model evaluation than any textbook."
ShowToc: false
ShowReadingTime: true
---

FootieM8 started as a class exercise: can the probabilistic models we study in econometrics actually predict football matches? The answer turned out to be yes — and also no, depending on what you mean by "predict."

---

### The architecture

The system combines two families of models. The first is probabilistic: Poisson regression and Dixon-Coles models that estimate goal-scoring rates for each team and derive match outcome probabilities from those rates. The second is machine learning: LightGBM and logistic regression trained on Elo ratings, recent form, and historical bookmaker odds.

The ensemble weights these families together using cross-validated calibration. Walk-forward evaluation prevents data leakage — the system never sees future data during training, not even implicitly through feature engineering.

Covering 25+ leagues across 30+ seasons means dealing with messy data: team name changes, league restructurings, missing fixtures, and the fact that Accrington Stanley in 1996 is not the same entity as Accrington Stanley in 2024.

---

### What actually worked

The Poisson and Dixon-Coles models are surprisingly robust. They capture the base rates well — home advantage, defensive strength, scoring trends — and produce well-calibrated probabilities. When they say a team has a 40% chance of winning, that team wins roughly 40% of the time.

Elo ratings, despite their simplicity, are the single best feature for ML models. Better than recent form, better than goals scored, better than anything derived from betting odds. The LightGBM ensemble adds marginal lift on top of the probabilistic models, mainly by capturing nonlinear interactions between team quality and venue effects.

---

### What didn't

Beating the market is a different problem than predicting outcomes. The models are well-calibrated, but prediction markets (Kalshi, in my case) are *also* well-calibrated. The edge, when it exists, is small — typically 1-3% on specific match types. After transaction costs and the platform's spread, most of that edge evaporates.

The honest conclusion: the models work as a prediction system. They don't work as a money machine. That's actually the more interesting finding — it's evidence that these markets are reasonably efficient, even for relatively obscure leagues.

---

### The meta-lesson

Building FootieM8 taught me more about model evaluation than any class. When you have skin in the game — even play money on Kalshi — you start caring about calibration, not just accuracy. You learn the difference between a model that's impressive on a test set and a model you'd actually bet on.

That distinction matters just as much in asset pricing, where the "bet" is a portfolio allocation and the "evaluation" is whether your Sharpe ratio survives out of sample.
