# quant-toolkit

Personal Python toolkit for conditional-density forecasting and risk-based trading signals on G8 FX, NQ, and Gold.
See `docs/methodology-references.md` for academic provenance.

---

## Roadmap

| Phase | Package | Based on | Status |
|-------|---------|----------|--------|
| 1 | `density-engine` | Adrian, Boyarchenko & Giannone (2019); Koenker & Bassett (1978); Chernozhukov, Fernandez-Val & Galichon (2010); Schmidt & Zhu (2016) | Scaffolded |
| 2 | `signal-layer` | Jorda (2005); Jorion (2007) | Scaffolded |
| 3 | `portfolio-layer` | Mean-variance and risk-parity portfolio construction | Scaffolded |

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

All code in this repository is original. Methodologies are grounded in published academic research.
See `docs/methodology-references.md` for full references.
