# BTCUSDT public klines

Public BTCUSDT USDT-M perpetual futures dataset prepared for reproducible backtests.

## Dataset

- Symbol: BTCUSDT
- Venue: Binance USDT-M perpetual futures
- Interval: 15m
- Timezone: UTC
- First kline open time: 2024-01-01 00:00:00 UTC
- Last kline open time: 2026-06-07 23:45:00 UTC
- Kline rows: 85,344
- Funding rows: 2,667
- Gap check: 0 missing 15m bars in the packaged file

## Files

- `BTCUSDT-15m.csv.gz` - compressed 15m OHLCV klines.
- `BTCUSDT-funding.csv.gz` - compressed BTCUSDT funding-rate records.
- `manifest.json` - source notes, date range, row counts, and SHA-256 checksums.

## Columns

Kline CSV columns:

```text
open_time,open,high,low,close,volume
```

`open_time` is Unix milliseconds in UTC.

## Sources

- Binance Futures REST API `/fapi/v1/klines`
- Binance Futures REST API `/fapi/v1/fundingRate`

This repository is for research and paper-trading/backtesting only. It is not investment advice.
