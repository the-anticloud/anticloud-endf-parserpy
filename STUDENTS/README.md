# Students — ENDF_PARSERPY

**Project:** ENDF_PARSERPY  
**Category:** NUCLEAR  
**Upstream:** https://github.com/IAEA-NDS/endf-parserpy  
**Pinned commit:** `e03429bf0b1163aa685e0d9b1c6d2cfbe9f6a622`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `a095e8cde306133c6011ff43d65147eacdca8808cea20d25d064560653dd8b95`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `e03429bf0b1163aa685e0d9b1c6d2cfbe9f6a622`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `a095e8cde306133c6011ff43d65147eacdca8808cea20d25d064560653dd8b95`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
