---
title: "Projects"
aliases: /projects
description: "Side projects and teaching tools"
tags: ["python", "machine-learning", "finance", "data-science"]
---

Where curiosity meets impatience.

---

### SpotiM8
`Python` `Pandas` `Spotify API` `Parquet`

A production-grade Python pipeline that treats my Spotify library as panel data. Syncs playlists, tracks, and artist metadata into tidy DataFrames, caches everything locally in Parquet, and maintains yearly archive playlists automatically. What started as curiosity about genre drift and listening patterns became a full sync engine with cron automation, streaming history analysis, and a notebook suite that doubles as a diary of how taste shifts under stress.

- Pandas-first interface over the Spotify Web API
- Incremental sync with smart cache invalidation
- Yearly archive playlists: Finds, Top, and Discovery per year
- Streaming history integration from Spotify data exports

Built because I wanted to ask questions about my own consumption data without trusting someone else's dashboard.

---

### ETFm8
`Python` `Machine Learning` `Robinhood API`

An automated ETF rebalancing system that generates trading orders from momentum, volatility, and drawdown signals. Scores positions, sizes allocations, detects market regimes, and outputs limit orders with optimal pricing. Optionally plugs into Robinhood for live portfolio sync.

- Signal-driven edge scoring with configurable weights
- Market regime detection for risk-on/risk-off switching
- Optional ML layer for position sizing and edge refinement
- Risk management: position limits, turnover caps, cash optimization

Born from wanting a systematic way to rebalance without pretending I can time anything.

---

### FootieM8
`Python` `LightGBM` `Dixon-Coles` `Kalshi API`

A research-grade football prediction system that combines probabilistic models (Poisson, Dixon-Coles) with machine learning (LightGBM, logistic regression) in a weighted ensemble. Covers 25+ leagues across 30+ seasons, runs walk-forward evaluation to prevent data leakage, and generates bet recommendations for Kalshi prediction markets.

- Elo ratings, form features, and bookmaker odds as inputs
- Ensemble of probabilistic and ML models with k-fold CV
- Time-aware evaluation: rolling windows, calibration metrics
- Automated bet generation with fuzzy team matching and risk caps

Started as a way to test whether the models I study in class hold up when the data fights back.

---

### M8MIX
`Python` `YouTube API` `FFmpeg`

A public domain music discovery and download pipeline for a YouTube channel. Automates the process of finding, downloading, and processing royalty-free music and creating visual content for uploads.

- Automated music library management and metadata tagging
- Video and VFX library organization
- YouTube API integration for channel management

Built to systematize creative work and learn media pipeline engineering.

---

### Financial ML Teaching Notebooks
`Python` `Jupyter` `scikit-learn`

Reusable Jupyter notebooks that try to make the math feel grounded:

- Visual bias-variance tradeoff
- Regularization as a form of belief-shrinkage
- How factor models sneak into ML regressions

Built while TA-ing at Chicago Booth and iterated in real classrooms. The goal is to leave students with code they can actually remix.
