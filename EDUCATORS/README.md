# Educators — STENOTYPE

**Project:** STENOTYPE  
**Category:** ELECTRICITY_MANAGEMENT  
**Upstream:** https://github.com/a-recknagel/stenotype  
**Pinned commit:** `d398a9b3939c08599d3bea362ff58e7ff9114325`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `3ad4cce711ddb0275656cdc832b341e90e6b0faef8ec23c287674d31c3efbde3`  
**Date:** October 2026

## Teaching with STENOTYPE

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `3ad4cce711ddb0275656cdc832b341e90e6b0faef8ec23c287674d31c3efbde3` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
