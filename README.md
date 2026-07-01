# mageos-data

Public aggregated perp DEX metrics powering [mage OS](https://cryptomage-mageos.pages.dev).

- `metrics.json` — per-venue average top-of-book spread (bps of mid) and funding APR (%)
  for BTC/ETH/SOL perps, over 24h and 7d windows.
- Sampled every 5 minutes from public venue APIs (keyless), aggregated hourly.
- Funding rates are normalized to hourly then annualized; `binance` is the CEX reference row.
- No positions, no account data, no secrets — aggregate public market data only.

Consumed via `https://raw.githubusercontent.com/coinmage777/mageos-data/main/metrics.json`.
Maintained automatically by the CryptoMage fleet infra.
