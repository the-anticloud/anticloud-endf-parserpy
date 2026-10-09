# Educators — ENDF_PARSERPY

**Project:** ENDF_PARSERPY  
**Category:** NUCLEAR  
**Upstream:** https://github.com/IAEA-NDS/endf-parserpy  
**Pinned commit:** `e03429bf0b1163aa685e0d9b1c6d2cfbe9f6a622`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `a095e8cde306133c6011ff43d65147eacdca8808cea20d25d064560653dd8b95`  
**Date:** October 2026

## Teaching with ENDF_PARSERPY

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `a095e8cde306133c6011ff43d65147eacdca8808cea20d25d064560653dd8b95` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
