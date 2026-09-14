# ohlcv-replay

> ohlcv · replay · fee

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

OHLCV replay engine — stub candles, fee model, equity.

## Features

- Default venue binance / BTCUSDT
- Built-in ema strategy plus paper mode
- Risk manager with daily-loss kill switch
- OHLCV store and SHA-256 stub candles
- Backtester with fill + fee model
- Click CLI: backtest, paper, status, orders

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd ohlcv-replay
python -m pip install -e .
python -m ohlcvreplay --help
```

## CLI Usage

```bash
ohlcvreplay backtest --bars 200
# Replay stub candles

ohlcvreplay paper
# Start a paper session

ohlcvreplay status
# Print engine state

ohlcvreplay orders
# List simulated fills
```

## Project Structure

```
ohlcvreplay/
  core/        engine + risk
  strategy/    grid / dca / ema hooks
  exchange/    stub order client
  data/        candles + backtest
  cli.py
tests/
```

## Configuration

See `ohlcvreplay/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `exchange` | `binance` | Venue id |
| `symbol` | `BTCUSDT` | Default pair |
| `strategy` | `ema` | Active strategy |
| `mode` | `paper` | paper or backtest |

## Tests

```bash
python -m pytest -q
```

## Background

Backtest people search ohlcv-replay before a framework name.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![ohlcv](https://img.shields.io/badge/ohlcv-111827?style=flat-square) ![replay](https://img.shields.io/badge/replay-111827?style=flat-square) ![ohlcv-replay](https://img.shields.io/badge/ohlcv%20replay-111827?style=flat-square) ![trading-bot](https://img.shields.io/badge/trading%20bot-111827?style=flat-square) ![crypto-trading](https://img.shields.io/badge/crypto%20trading-111827?style=flat-square) ![binance](https://img.shields.io/badge/binance-111827?style=flat-square) ![defi](https://img.shields.io/badge/defi-111827?style=flat-square) ![algorithmic-trading](https://img.shields.io/badge/algorithmic%20trading-111827?style=flat-square)

`ohlcv` `replay` `ohlcv-replay` `trading-bot` `crypto-trading` `binance` `defi` `algorithmic-trading` `quantitative-finance` `open-source` `python`

Search: ohlcv-replay · ohlcv · replay · fee · OHLCV replay engine — stub candles, fee model, equity.

---

<sub>OHLCV replay engine — stub candles, fee model, equity.</sub>
