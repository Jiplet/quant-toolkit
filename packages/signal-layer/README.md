# signal-layer

Phase 2 package. Translates density estimates into actionable directional and volatility signals.

## Purpose

Builds on density-engine outputs to generate regime-aware signals for entry, sizing, and
risk management. Covers FX volatility modelling and forward quantile projection.

## Source mapping

| Lafarguette repo | Method | Phase |
|-----------------|--------|-------|
| `varfxi` | FX volatility intervention model (VAR-based FX impact estimation) | Phase 2 |
| `quantileproj` | Quantile projection for forward-looking distribution paths | Phase 2 |

Status: queued for Phase 2.

## Planned modules

- `signal_layer.varfxi` - VAR-based FX volatility and regime signal
- `signal_layer.quantileproj` - forward quantile path projection
- `signal_layer.signals` - unified signal interface (direction, strength, regime)

## Status

Scaffold only. No code ported yet.
