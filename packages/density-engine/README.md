# density-engine

Phase 1 package. Conditional density estimation for FX, NQ, and Gold return distributions.

## Purpose

Fits conditional return densities using growth-at-risk and conditional quantile sampling
methods. Produces distribution parameters (skewness, tail risk, mode) that feed the
signal-layer.

## Based on

- Adrian, T., Boyarchenko, N. & Giannone, D. (2019). "Vulnerable Growth". *American Economic Review* 109(4), 1263-1289. -- conditional density forecasting via quantile regression.
- Koenker, R. & Bassett, G. (1978). "Regression Quantiles". *Econometrica* 46(1), 33-50. -- quantile regression core.
- Chernozhukov, V., Fernandez-Val, I. & Galichon, A. (2010). "Quantile and Probability Curves Without Crossing". *Econometrica* 78(3), 1093-1125. -- monotonicity correction.
- Schmidt, L. & Zhu, Y. (2016). "Quantile Spacings: A Simple Method for the Joint Estimation of Multiple Quantiles". -- density recovery from conditional quantiles.

See `docs/methodology-references.md` for full citations.

## Planned modules

- `density_engine.gar` - quantile regression models for return distribution
- `density_engine.cqsampling` - density recovery from conditional quantiles
- `density_engine.fit` - unified fit/predict interface

## Status

Scaffold only. No code written yet. Awaiting Jacob approval to begin Phase 1.
