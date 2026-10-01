---
title: "Projects"
aliases: /projects
description: "Side projects"
---

{{< jumplinks "Finance and Machine Learning" "Just for Fun" >}}

## Finance and Machine Learning

- **Prediction Market Price Discovery.** A study of the same events traded on Polymarket and Kalshi. I collected about 90,000 Polymarket and 550,000 Kalshi markets, matched 759 identical contracts across the two using text similarity, and measured how far their prices drift apart, how quickly the gap closes, and which platform moves first. In this sample, price gaps close with a half-life of about two hours, and Polymarket leads most of the price discovery.
- **Black-Litterman with Machine Learning Views.** Black-Litterman portfolios usually need an investor to supply views on expected returns. Here the views come from LightGBM and random forest forecasts instead, tested on Dow Jones stocks from 2019 to 2023 against market-cap and equal-weighted portfolios.
- **ETFm8.** A small tool for rebalancing an ETF portfolio using simple signals, with an optional Robinhood connection.

---

## Just for Fun

- **Department of Unnecessary Football.** Football analysis I do for fun.
    - **World Cup 2026 by club and league.** I rebuilt every player's minutes at the 2026 World Cup from match events (102 of 104 matches, 1,248 players) and broke down contributions by club, league, stage, and position. My reconstruction matches ESPN's published minutes for 1,237 players.
    - **FPL Lab.** A Fantasy Premier League system I am running live in 2026-27. A LightGBM model forecasts player points, and an integer program picks the squad and weekly transfers. In backtests, it has not beaten FPL's own forecasts.
- **SpotiM8.** Pulls my Spotify library and listening history into pandas and Parquet, keeps yearly archive playlists updated, and has a small Streamlit dashboard.
- **M8MIX.** Finds public-domain music recordings on the Internet Archive, the Library of Congress, and Wikimedia Commons, checks their rights status, analyzes the audio with librosa, and builds mixes with FFmpeg for a YouTube channel. The library has about 4,200 tracks so far, and three mixes are published.
