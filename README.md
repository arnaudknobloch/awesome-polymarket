# Awesome Polymarket

> A curated, link-verified list of tools, libraries, bots, datasets, and resources for the Polymarket ecosystem.

Polymarket is a prediction market where users trade on the outcome of future events. This list collects the software built around it: whale trackers, copy-trading engines, market-making bots, SDKs, historical datasets, and MCP servers for AI agents.

**Every link here was checked on 2026-08-11.** Entries that 404, resolve to a parked domain, or point at a Chrome Web Store page that no longer exists have been removed rather than carried forward. If you find a dead link, [open an issue](../../issues).

## Contents

- [Official Resources](#official-resources)
- [Whale Tracking](#whale-tracking)
- [Trader Scoring & Wallet Analysis](#trader-scoring--wallet-analysis)
- [General Analytics](#general-analytics)
- [Copy Trading](#copy-trading)
- [Trading Bots & Automation](#trading-bots--automation)
- [Arbitrage & Cross-Platform](#arbitrage--cross-platform)
- [Alerts](#alerts)
- [API Libraries & SDKs](#api-libraries--sdks)
- [Data APIs & Datasets](#data-apis--datasets)
- [AI Agents & MCP Servers](#ai-agents--mcp-servers)
- [Browser Extensions](#browser-extensions)
- [Directories](#directories)
- [Educational Resources](#educational-resources)
- [Community](#community)
- [Contributing](#contributing)

## Official Resources

- [Polymarket](https://polymarket.com/) - The platform itself.
- [Polymarket Documentation](https://docs.polymarket.com/) - Developer documentation and API reference.
- [Polymarket 101](https://docs.polymarket.com/polymarket-101) - Official introduction to how the markets work.
- [API Quickstart](https://docs.polymarket.com/quickstart) - Getting started with programmatic trading.
- [Polymarket News](https://news.polymarket.com/) - Official news and market commentary.
- [Polymarket on GitHub](https://github.com/Polymarket) - Official repositories.
- [Gamma API](https://gamma-api.polymarket.com/) - Market metadata and event data.
- [CLOB API](https://clob.polymarket.com/) - Central limit order book, order placement and market data.

## Whale Tracking

- [PolyTrack](https://polytrack.org/) - Whale tracking with real-time alerts, leaderboards, P&L tracking, and trader profiles.
- [Polywhaler](https://polywhaler.com/) - Tracks $10k+ trades with insider activity detection.
- [PolyTrace](https://polytrace.app) - Free tracker covering every $1,000+ fill, each trade shown with the wallet's P&L, sample-aware win rate, and 0-100 score. Public methodology.
- [Whalefax](https://whalefax.com/) - Whale leaderboard with a full history rebuild that recovers unredeemed losing positions other trackers miss. Free, no signup.
- [0xinsider](https://0xinsider.com/) - Terminal streaming large Polymarket and Kalshi trades across 7,000+ tracked traders, with trader grades, 40+ quant metrics, and signal scoring. REST API and MCP server.
- [EdgeMarket](https://edgemarket.co/) - Whale radar over 144k tracked Polymarket wallets, ranked by measured alpha rather than displayed P&L, plus a public register of 5-minute BTC/ETH/SOL/XRP calls confirmed at T+180s with misses included, and funding/OI/liquidations on four venues. Free tier for the register; live signals and Telegram alerts from $39/mo.
- [WhaleTracker](https://whale-tracker-lovat.vercel.app) - Free real-time whale dashboard with $10K+ trade filtering, hot markets, and buy/sell bias analytics.

## Trader Scoring & Wallet Analysis

Tools that try to separate skill from luck before you follow a wallet.

- [PolyScore](https://polytrading.app) - Skill-vs-luck wallet ratings (0-100) built from full on-chain trade history. Free wallet check and a scored leaderboard with bots filtered out.
- [OVERROUND](https://overround.pro/) - Grades wallets on price-relative accuracy over independent resolved events, and publishes a graded ledger of every alert sent, losses included.
- [Cobia Picks](https://cobiapicks.com) - Scores signals from proven wallets with a trained model, then grades every pick in public. 2,000+ resolved, losses included.
- [polymarket-honest-tools](https://github.com/yntymacho/polymarket-honest-tools) - Copy-trade validator that tests whether a wallet's edge survives realistic fills, fees, and out-of-sample data before you copy it.
- [polymarket-pnl](https://github.com/LuciferForge/polymarket-pnl) - Command-line P&L breakdown for any wallet, no API keys required.

## General Analytics

- [Polyguana](https://polyguana.com/) - Analytics dashboard with trader leaderboards, whale tracking, portfolio performance, and real-time market data.
- [protodex.io](https://protodex.io) - Free screener and data API indexing 19,300+ markets.
- [TrueOdds](https://trueodds.win/) - AI fair-value engine, live signal feeds, whale and insider radar, and a trader screener over thousands of wallets.
- [Boosted Trading](https://boosted.trading) - Trading desk with in-app execution, P&L journaling, leaderboards, charts, quant signals, and risk management tools.
- [PolyMind](https://polyminds.netlify.app/) - Alert platform with 12 signal types (whale bets, volume spikes, coordinated wallets, reversals, late money) and multi-model AI analysis.
- [Airavat](https://airavat.xyz/) - Trading analytics with on-chain trader scoring, real-time trade filters, and paper or live auto-trade execution.
- [Dune Analytics](https://dune.com/browse/dashboards?q=polymarket) - Community dashboards for volume, open interest, and user analytics.
- [ClearMarket](https://github.com/JDSource/clearmarket) - Intelligence layer adding parsed resolution logic, catalyst calendars, and cross-platform mapping to raw Polymarket and Kalshi data.

## Copy Trading

- [PredCopy](https://predcopy.com/) - Whale tracking and composite trader scoring paired with an execution engine that mirrors a followed wallet under configurable bet sizing, max exposure, and stale position exit rules. Telegram alerts and an MCP server.
- [CopyTrail](https://copytrail.org) - Mirrors top traders' on-chain fills into your own wallet, with a free paper mode to verify fills before going live and an ECIES-encrypted trading key.
- [FrenFlow](https://www.frenflow.com/copytrading) - Non-custodial block-0 copy trading across Polymarket and Kalshi, mirroring a leader's fills in the same block via mempool detection. Per-trade stake caps and HFT-bot flagging.
- [Polyman](https://t.me/PolymanApp_bot) - Telegram Mini App and web app for copy-trading top traders with AI-scored signals.
- [Polycool](https://polycool.live/) - Tracks the top 0.5% of wallets and pushes big trades to Telegram for copy-trading.

## Trading Bots & Automation

### Official

- [Polymarket Agents](https://github.com/Polymarket/agents) - Official AI agent framework with LLM integration and a modular architecture.
- [poly-market-maker](https://github.com/Polymarket/poly-market-maker) - Official CLOB market maker with bands or AMM strategy, and Docker support.

### Market Making

- [poly-maker](https://github.com/warproxxx/poly-maker) - Automated market-making bot with Google Sheets configuration and position merging.
- [polymarket-marketmaking](https://github.com/elielieli909/polymarket-marketmaking) - Band-based market-making bot with automated order management.
- [polymm](https://github.com/kachence/polymm) - Sports market-making and arbitrage bot in Python. De-vigs sportsbook odds, quotes limit orders, and hedges to lock the arb.

### Strategy & Execution

- [predtools](https://predtools.com/) - Source-available trading bots for Polymarket and Kalshi with a strategy library, sold as one-time purchases.
- [polymarket-bot-lab](https://github.com/oraclemangle/polymarket-bot-lab) - Lab of 11 candidate strategies with CLOB clients, fee models, a backtest engine, and risk gates. Publishes confidence intervals and the strategies that lost money.
- [antflow](https://antflow.live) - Autonomous trading bot with risk guardrails and disciplined exits, results shown on a public live wallet rather than a backtest.
- [polymarket-settlement-bot](https://github.com/LuciferForge/polymarket-settlement-bot) - Auto-redeems resolved positions back to USDC.

### Specialized

- [Polymarket Weather Command Center](https://github.com/testedmedia/polymarket-weather-command-center) - Apache-2.0 dashboard for temperature markets: multi-model forecasts, live ASOS/METAR airport observations, bucket probabilities, and market edge across 41 cities.
- [WinWeatherBot](https://winweatherbot.com) - Automated weather trading with a 138-model forecast ensemble, correlation-aware sizing, and sub-200ms execution.
- [polymarket-odds-scanner](https://github.com/LuciferForge/polymarket-odds-scanner) - Finds mispriced sports markets by comparing Polymarket prices against sportsbook odds.

## Arbitrage & Cross-Platform

- [PredRadar](https://predradar.com/) - Cross-platform aggregator for Polymarket, Kalshi, and Betfair with live prices, an arbitrage scanner, a JSON API, and an MCP server.
- [OddsShift](https://oddsshift.com/) - Comparison across Polymarket and Kalshi with AI analysis of price divergences, arbitrage detection, and smart money tracking.
- [PredMart](https://predmart.com) - Non-custodial margin account: trade with up to 5x leverage, or borrow USDC against prediction-market shares you already hold. Built on Polygon.

## Alerts

- [PolyAlertHub](https://polyalerthub.com/) - Alerts on profitable traders, whales, and market trends, delivered by email or Telegram.
- [ScoreEdge](https://scoreedge.app) - Sports alerts for Polymarket and Kalshi traders. Rules on score changes, lead flips, and play-by-play events, pushed before markets reprice.
- [SignalRadar](https://github.com/vahnxu/signalradar) - Zero-dependency Python CLI that monitors markets for probability changes and pushes threshold alerts by webhook, Telegram, or file.

## API Libraries & SDKs

### Python

- [py-clob-client](https://pypi.org/project/py-clob-client/) - Official Python client for the CLOB, with order execution and market data.
- [polymarket-apis](https://pypi.org/project/polymarket-apis/) - Unified APIs with Pydantic models across CLOB, Gamma, Data, Web3, WebSocket, and GraphQL.
- [polymarket-pandas](https://pypi.org/project/polymarket-pandas/) - Pandas-native SDK wrapping every Polymarket API with DataFrame returns, pandera schemas, async support, and pagination.
- [polymarket-api-python](https://pypi.org/project/polymarket-api-python/) - Typed client to read Gamma markets, snapshot and stream the order book, and place orders with idempotent client order ids.

### JavaScript / TypeScript

- [@polymarket/clob-client](https://www.npmjs.com/package/@polymarket/clob-client) - Official CLOB client with order placement, market data, and WebSocket support.
- [@polymarket/sdk](https://www.npmjs.com/package/@polymarket/sdk) - Official SDK for proxy wallet interactions and trading.
- [@polymarket/embeds](https://www.npmjs.com/package/@polymarket/embeds) - Official embeddable web components for markets.
- [@polybased/sdk](https://www.npmjs.com/package/@polybased/sdk) - TypeScript toolkit with real-time data and WebSocket streams.
- [polymarket-data](https://www.npmjs.com/package/polymarket-data) - Community TypeScript client for public data with type safety.
- [@dicedhq/polymarket](https://jsr.io/@dicedhq/polymarket) - TypeScript client covering the CLOB and Gamma.

### Rust

- [polyfill-rs](https://github.com/floor-licker/polyfill-rs) - High-performance Rust client with latency-optimized data structures, zero-allocation hot paths, and CLOB support.

### Agent Framework Plugins

- [@theschein/plugin-polymarket](https://www.npmjs.com/package/@theschein/plugin-polymarket) - ElizaOS integration for AI agent trading.
- [@goat-sdk/plugin-polymarket](https://www.npmjs.com/package/@goat-sdk/plugin-polymarket) - GOAT SDK plugin for market data and betting.

## Data APIs & Datasets

- [PMXT](https://github.com/pmxt-dev/pmxt) - Open-source unified API for prediction market data across exchanges.
- [Marketlens](https://marketlens.trade/) - Tick-level historical order book data and trades, with a Python SDK and a backtesting REST API.
- [Telonex](https://telonex.io/) - Tick-level historical trades, quotes, order books, and on-chain fills via REST API and Python SDK.
- [polymarket-api](https://github.com/LuciferForge/polymarket-api) - Free, open-source REST API serving 10M+ historical price snapshots.
- [polymarket-historical-data](https://github.com/LuciferForge/polymarket-historical-data) - Open historical price dataset, 19M+ snapshots across 19,300+ markets.
- [polymarket-canary-tape](https://huggingface.co/datasets/oraclemangle/polymarket-canary-tape) - CC-BY-4.0 historical tape: 271M CEX trades and ~61M Polymarket WebSocket events with a dual-vantage overlap window for latency research.
- [Matched book sample](https://huggingface.co/datasets/Coyevans/mlb-polymarket-kalshi-matched-book-sample) - Order book sample labeled with settled outcomes, cross-matched against Kalshi.
- [Bitquery](https://bitquery.io/) - On-chain analytics and smart contract events for the Polymarket contracts on Polygon.

## AI Agents & MCP Servers

- [polymarket-mcp](https://github.com/LuciferForge/polymarket-mcp) - Live market data exposed as MCP tools for Claude and other agents.
- [Predge Whale Data MCP](https://github.com/predgeAI/whale-data-mcp) - MCP server exposing whale trades, win-rate wallet leaderboards, smart-money consensus, and signed settled outcomes. Pay-per-call USDC, no API keys.
- [Predge Whale Data](https://data.predge.io) - Outcome-verified whale intelligence for agents, with ed25519-signed settled market and sports outcomes verifiable offline.
- [oracle3](https://github.com/YichengYang-Ethan/oracle3) - Autonomous trading agent with Wang Transform pricing, eight constraint-based arbitrage strategies, and Kelly-sized execution. Apache 2.0, with an SSRN working paper.
- [Lightning Rod Foresight Models](https://www.lightningrod.ai/models) - Forecasting models behind an OpenAI-compatible API.

## Browser Extensions

- [PolySmart](https://chromewebstore.google.com/detail/polysmart-%E2%80%94-smart-money-a/jkbeggmpenineniihnhhabjgamcigoho) - Smart money analyzer with whale tracking, entry price detection, and holder win-rate scoring on every market page.
- [PolyChart](https://chromewebstore.google.com/detail/polychart-candlestick-cha/gdfcfkbghfcpbepdeehfnofadgmjbmio) - Candlestick charts with technical analysis overlays.
- [PolySniper](https://chromewebstore.google.com/detail/polysniper-polymarket-arb/mljgjdaaopkcipmkdeafdopnopbaompo) - Real-time negRisk arbitrage scanner with CLOB-verified signals, spread calculation, and order book depth.

## Directories

- [pm.wiki](https://pm.wiki/) - Independent prediction market directory covering 350+ tools and platforms with side-by-side comparisons.
- [Polymark.et](https://polymark.et/) - Directory of Polymarket tools and products.
- [LaunchPoly](https://launchpoly.com) - Community-voted directory of bots, analytics, alerts, trackers, and extensions.

## Educational Resources

- [Polymarket Academy](https://polymarketacademy.com/) - Copy trading guides with bot reviews, security comparisons, and step-by-step tutorials.
- [Prediction Market FAQ](https://astralcodexten.substack.com/p/prediction-market-faq) - Scott Alexander's overview of how prediction markets work and what they are good for.
- [The Passage of Polymarket](https://astralcodexten.substack.com/p/the-passage-of-polymarket) - On Polymarket's rise.
- [Market Mechanics](https://manifoldmarkets.substack.com/p/above-the-fold-market-mechanics) - How prediction market mechanics actually function.

## Community

- [Polymarket on X](https://twitter.com/Polymarket) - Official account.
- [Polymarket Discord](https://discord.gg/polymarket) - Official Discord.
- [r/Polymarket](https://reddit.com/r/polymarket) - Reddit community.
- [0xperp's Polymarket List](https://twitter.com/i/lists/1684720466500431872) - Curated list of Polymarket traders and analysts.

## Contributing

Pull requests are welcome. Two rules:

1. **The link must work.** Every entry is checked before merging, and re-checked periodically. Chrome Web Store links need the full extension ID, not just a slug.
2. **Say what it does, concretely.** "Real-time AI-powered insights" tells a reader nothing. What does it track, what does it output, is it free?

Disclose it if you built the tool. That is fine, it just needs saying.

## Credits

This list started as a cleanup of [Awesome-Polymarket-Tools](https://github.com/harish-garg/Awesome-Polymarket-Tools) by Harish Garg (CC0), and merges entries from contributor pull requests that were left open there. Broken and unverifiable entries were dropped in the process.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.
