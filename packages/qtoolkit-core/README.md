# qtoolkit-core

Shared foundation package for quant-toolkit. No internal workspace dependencies.

## Purpose

Provides the shared primitives used by all other packages:
- OHLC data types and structures
- Data loaders: yfinance (price) and FRED (macro)
- Configuration management (API keys, ticker lists, factor set)
- Common utilities: logging, date handling, validation

## Based on

No specific method paper. Purpose-built shared infrastructure for the toolkit.

## Planned modules

- `qtoolkit_core.types` - OHLC dataclasses, factor set types
- `qtoolkit_core.loaders` - yfinance + FRED data fetch
- `qtoolkit_core.config` - workspace configuration
- `qtoolkit_core.utils` - shared helpers

## Status

Scaffold only. No code written yet.
