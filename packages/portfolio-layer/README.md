# portfolio-layer

Phase 3 package. Density-informed position sizing and portfolio construction.

## Purpose

Uses forward density projections to construct risk-based position sizes and
portfolio allocations. Covers scenario-weighted outcomes and drawdown budgeting
for the core-satellite framework (indices core, active FX/futures satellite).

## Source mapping

| Lafarguette repo | Method | Phase |
|-----------------|--------|-------|
| `densproj` | Density projection: scenario weighting over forward return distributions | Phase 3 |
| `gic-junior-quant-pc-recruitment` | Portfolio construction and risk decomposition examples | Phase 3 |

Status: queued for Phase 3.

## Planned modules

- `portfolio_layer.densproj` - forward density projection and scenario weighting
- `portfolio_layer.sizing` - risk-based position sizing (Kelly variants, VaR-scaled)
- `portfolio_layer.portfolio` - portfolio construction and allocation

## Status

Scaffold only. No code ported yet.
