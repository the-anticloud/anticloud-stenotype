# Ethics — STENOTYPE

**Project:** STENOTYPE  
**Category:** ELECTRICITY_MANAGEMENT  
**Upstream:** https://github.com/a-recknagel/stenotype  
**Pinned commit:** `d398a9b3939c08599d3bea362ff58e7ff9114325`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `3ad4cce711ddb0275656cdc832b341e90e6b0faef8ec23c287674d31c3efbde3`  
**Date:** October 2026

## Position

STENOTYPE is packaged for offline deployment with a verifiable audit trail. The
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
