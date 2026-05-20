# density-engine

Phase 1 package. Conditional density estimation for FX, NQ, and Gold return distributions.

## Purpose

Fits conditional return densities using growth-at-risk and conditional quantile sampling
methods. Produces distribution parameters (skewness, tail risk, mode) that feed the
signal-layer.

## Source mapping

| Lafarguette repo | Method | Phase |
|-----------------|--------|-------|
| `gar` | Growth-at-Risk: conditional quantile fitting via quantile regression | Phase 1 |
| `cqsampling` | Conditional quantile sampling to recover full density | Phase 1 |

Status: queued for Phase 1 porting, pending Jacob approval.

## Planned modules

- `density_engine.gar` - quantile regression models for return distribution
- `density_engine.cqsampling` - density recovery from conditional quantiles
- `density_engine.fit` - unified fit/predict interface

## Status

Scaffold only. No code ported yet. Awaiting Jacob approval to begin Phase 1.
