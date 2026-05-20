# portfolio-layer

Phase 3 package. Density-informed position sizing and portfolio construction.

## Purpose

Uses forward density projections to construct risk-based position sizes and
portfolio allocations. Covers scenario-weighted outcomes and drawdown budgeting
for the core-satellite framework (indices core, active FX/futures satellite).

## Based on

Standard portfolio construction methods: mean-variance optimisation and risk-parity allocation.
No specific method paper applies at this stage. See `docs/methodology-references.md` for the
VaR framework (Jorion, 2007) that informs the risk-sizing approach.

## Planned modules

- `portfolio_layer.densproj` - forward density projection and scenario weighting
- `portfolio_layer.sizing` - risk-based position sizing (Kelly variants, VaR-scaled)
- `portfolio_layer.portfolio` - portfolio construction and allocation

## Status

Scaffold only. No code written yet.
