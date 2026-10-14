# Build and Test

**Project:** `STENOTYPE`
**Upstream:** https://github.com/StevenTammen/stenotype
**License:** GPL

## Quick Start

```bash
git clone https://github.com/StevenTammen/stenotype
cd stenotype
pip install -r requirements-anticloud.txt
python anticloud_main.py --offline --pax-local
```

## Anticloud Improvements Applied

1. PAX L5 Narrow L2 General 27B local load forecasting and fault prediction — edge deployment
2. AIOSS tamper-evident grid event log (NERC CIP aligned)
3. AES-256 encryption for all metering and SCADA data
4. Single-binary EMS deployment on utility substation hardware
5. Zero-cloud: all analytics and control logic run on local servers
6. GPU/CPU equalizer: real-time inference on edge GPU or CPU
7. Offline demand response optimization replacing cloud DR APIs
8. Open IEC 61968/61970 CIM integration replacing proprietary SCADA middleware

## Benchmark Targets

| Metric | Target |
| --- | --- |
| Latency | Primary inference task: <5s on CPU, <1s on GPU |
| Throughput | Batch processing: >100 items/hour on single CPU server |
| Memory | <8GB RAM for standard deployment |
| Accuracy | Task-specific accuracy within 5% of cloud-API baseline |

## Build Status

Not yet measured. Run verified build and record actual figures above.
