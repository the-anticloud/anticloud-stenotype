# Students — STENOTYPE

**Project:** STENOTYPE  
**Category:** ELECTRICITY_MANAGEMENT  
**Upstream:** https://github.com/a-recknagel/stenotype  
**Pinned commit:** `d398a9b3939c08599d3bea362ff58e7ff9114325`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `3ad4cce711ddb0275656cdc832b341e90e6b0faef8ec23c287674d31c3efbde3`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `d398a9b3939c08599d3bea362ff58e7ff9114325`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `3ad4cce711ddb0275656cdc832b341e90e6b0faef8ec23c287674d31c3efbde3`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
