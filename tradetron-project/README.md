# Tradetron Project

Cloud workspace for Tradetron strategies (NSE / BSE / MCX).

| Folder | Contents |
|---|---|
| `strategies/` | Exported Tradetron strategy definitions — one sub-folder per strategy family |
| `backtests/` | Backtest results (trades, P&L, drawdown) as CSV / JSON |
| `analysis/` | Python scripts — variant comparison, charges (STT, GST, stamp duty, SEBI fee) and slippage adjustment |
| `reports/` | Generated summaries and charts |

## Strategy register

| Strategy | Tradetron ID | Underlying | Status |
|---|---|---|---|
| Robo Trading Positional | 8858077 | — | — |
| Robo Hedge First SENSEX TGT 60 / 70 / 80 / 90 | 999452230 / 999452234 / 999452246 / 999452254 | SENSEX | — |
| SX Sell CE PE At 300 (AlgoTest port) | 999465614 | SENSEX | — |

## Rules

- **Never commit secrets** — broker API keys, Kotak Neo passwords, TOTP seeds, Tradetron tokens.
- NSE/BSE F&O backtests on Tradetron need data at least 35 days old.
- Every strategy change gets a commit message saying *what* changed (e.g. "TGT 80 → 90").
