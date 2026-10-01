---
title: "Projects"
aliases: /projects
description: "Side projects"
---

### Prediction Market Price Discovery

A study of the same events traded on Polymarket and Kalshi. I collected about 90,000 Polymarket and 550,000 Kalshi markets, matched 759 identical contracts across the two using text similarity, and measured how far their prices drift apart, how quickly the gap closes, and which platform moves first. In this sample, price gaps close with a half-life of about two hours, and Polymarket leads most of the price discovery.

### Black-Litterman with Machine Learning Views (2024)

Black-Litterman portfolios usually need an investor to supply views on expected returns. Here the views come from LightGBM and random forest forecasts instead, tested on Dow Jones stocks from 2019 to 2023 against market-cap and equal-weighted portfolios.

### ETFm8

A small tool for rebalancing an ETF portfolio using simple signals, with an optional Robinhood connection.

### SpotiM8

Pulls my Spotify library and listening history into pandas and Parquet, keeps yearly archive playlists updated, and has a small Streamlit dashboard.

### M8MIX

Finds public-domain music recordings on the Internet Archive, the Library of Congress, and Wikimedia Commons, checks their rights status, analyzes the audio with librosa, and builds mixes with FFmpeg for a YouTube channel. The library has about 4,200 tracks so far, and three mixes are published.
