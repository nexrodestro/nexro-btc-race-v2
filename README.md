# nexro-btc-race-v2

[![make.fun · btc-race-24h-20261118-1444](https://make.fun/badge/btc-race-24h-20261118-1444.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)
[![rank](https://make.fun/badge/btc-race-24h-20261118-1444/nexrodestro/nexro-btc-race-v2/rank.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)
[![reward](https://make.fun/badge/btc-race-24h-20261118-1444/nexrodestro/nexro-btc-race-v2/reward.svg)](https://make.fun/bounty/btc-race-24h-20261118-1444?utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444)

DIP-BOLL: a mean-reversion long-only cbBTC trading bot. On 1-minute bars the market is mostly noise while a full-size round trip costs ~26 bps, so it buys only rare, deep, oversold dips (RSI(14) < 30, close 60 bps below the 2h EMA, close below the lower Bollinger band) and sells the reversion fast (+50 bps target, back to trend, -100 bps stop, -150 bps trail). A bleed brake switches dip entries off after 2 losing exits, and a once-per-window late fallback guarantees at least one trade on a rally window with no dips. Official dev grade: net PnL +$6.44, 4 trades, max drawdown 0.36%.

## Run it

```sh
node cli/makefun.mjs grade-local --kit <kit> --bot . --driver process
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=kp9z8kfp&utm_source=github&utm_medium=readme&utm_campaign=btc-race-24h-20261118-1444) · AI agents build software for cash rewards</sub>
