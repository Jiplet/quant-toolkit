# quant-toolkit

Conditional-density forecasting and risk-based signals for G8 FX, NQ, and Gold.
Methodologies rewritten from IMF quant research for discretionary retail swing and intraday use.
See `docs/source-attribution.md` for academic provenance.

---

## Roadmap

| Phase | Package | Maps from (Lafarguette) | Status |
|-------|---------|------------------------|--------|
| 1 | `density-engine` | `gar` + `cqsampling` | Scaffolded, awaiting approval to port |
| 2 | `signal-layer` | `varfxi` + `quantileproj` | Scaffolded |
| 3 | `portfolio-layer` | `densproj` + `gic-junior-quant-pc-recruitment` | Scaffolded |

---

## Trading Universe

**FX (G8):** USDJPY, EURUSD, GBPUSD, USDCHF, AUDUSD, NZDUSD, USDCAD, EURJPY, GBPJPY

**Futures:** NQ (Nasdaq-100 E-mini), Gold (GC)

---

## Macro Factor Set

| Factor | Description |
|--------|-------------|
| US 2Y | US 2-year Treasury yield |
| US 10Y | US 10-year Treasury yield |
| VIX | CBOE Volatility Index |
| DXY | US Dollar Index |

---

## Data Sources

- **OHLC price data:** yfinance
- **Macro factors:** FRED (Federal Reserve Economic Data)

---

## Output Destinations (planned)

- Telegram alerts (via bot)
- Notion signal log
- n8n orchestration workflows

---

## Stack

- Python 3.12
- uv (workspace / dependency management)
- ruff (linting and formatting)
- pytest (testing)

---

## Package Layout

```
packages/
  qtoolkit-core/       # Shared: data loaders, OHLC types, config
  density-engine/      # Phase 1: conditional density estimation
  signal-layer/        # Phase 2: FX volatility and quantile projection signals
  portfolio-layer/     # Phase 3: density projection and portfolio construction
```

---

## Attribution

All code in this repository is original. Methodologies are adapted from published academic research
by Romain Lafarguette and co-authors at the IMF. Methodological credit is preserved in module
docstrings where applicable. See `docs/source-attribution.md` for per-repo license status.
