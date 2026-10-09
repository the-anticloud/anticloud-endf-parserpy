# Ethics — ENDF_PARSERPY

**Project:** ENDF_PARSERPY  
**Category:** NUCLEAR  
**Upstream:** https://github.com/IAEA-NDS/endf-parserpy  
**Pinned commit:** `e03429bf0b1163aa685e0d9b1c6d2cfbe9f6a622`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `a095e8cde306133c6011ff43d65147eacdca8808cea20d25d064560653dd8b95`  
**Date:** October 2026

## Position

ENDF_PARSERPY is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
