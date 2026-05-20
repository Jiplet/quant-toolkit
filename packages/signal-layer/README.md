# signal-layer

Phase 2 package. Translates density estimates into actionable directional and volatility signals.

## Purpose

Builds on density-engine outputs to generate regime-aware signals for entry, sizing, and
risk management. Covers FX volatility modelling and forward quantile projection.

## Based on

- Jorda, O. (2005). "Estimation and Inference of Impulse Responses by Local Projections". *American Economic Review* 95(1), 161-182. -- event-conditional forward quantile paths via local projections.
- Jorion, P. (2007). *Value at Risk: The New Benchmark for Managing Financial Risk*. 3rd ed., McGraw-Hill. -- VaR framing for risk-based signal thresholds.

See `docs/methodology-references.md` for full citations.

## Planned modules

- `signal_layer.varfxi` - VAR-based FX volatility and regime signal
- `signal_layer.quantileproj` - forward quantile path projection
- `signal_layer.signals` - unified signal interface (direction, strength, regime)

## Status

Scaffold only. No code written yet.
