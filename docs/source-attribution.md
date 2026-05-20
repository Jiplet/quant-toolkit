# Source Attribution

All code in quant-toolkit is original. The methodologies are adapted from published
academic and applied research by Romain Lafarguette and co-authors, primarily during
his tenure at the IMF.

Code is rewritten, not copied. Methodological credit is preserved in module docstrings
where applicable.

---

## Source Repositories Under Consideration

| Repo | Author | License | Phase | Status |
|------|--------|---------|-------|--------|
| `gar` | Lafarguette | TODO: check | Phase 1 | Queued for porting |
| `cqsampling` | Lafarguette | TODO: check | Phase 1 | Queued for porting |
| `varfxi` | Lafarguette | TODO: check | Phase 2 | Queued for porting |
| `quantileproj` | Lafarguette | TODO: check | Phase 2 | Queued for porting |
| `densproj` | Lafarguette | TODO: check | Phase 3 | Queued for porting |
| `gic-junior-quant-pc-recruitment` | Lafarguette | TODO: check | Phase 3 | Queued for porting |
| `granulariv` | Lafarguette | TODO: check | Tier 2 | May lift selectively |
| `plswrapper` | Lafarguette | TODO: check | Tier 2 | May lift selectively |
| `clusterwrapper` | Lafarguette | TODO: check | Tier 2 | May lift selectively |
| `robustdensity` | Lafarguette | TODO: check | Tier 2 | May lift selectively |

GitHub profile: https://github.com/romainlafarguette

---

## License Checklist (pre-porting)

Before any code is ported from a source repo:

1. Confirm the repo has an explicit open-source license (MIT, Apache 2.0, BSD, GPL, etc.)
2. If GPL, assess whether the copyleft terms are compatible with keeping this repo private
3. If no license present, do not port code without explicit written permission from Lafarguette
4. Record the confirmed license in the table above
5. Add a methodological attribution comment in the relevant module docstring

---

## Note on Rewriting vs Copying

Porting in this project means: understand the method, rewrite in modern Python (3.12),
adapt for retail trading use cases (OHLC data, G8 FX tickers, NQ, Gold), and discard
IMF-specific data pipeline assumptions. The output is methodologically derived, not a
code fork.
