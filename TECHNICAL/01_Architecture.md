# Technical Architecture — STENOTYPE

**Upstream:** [https://github.com/StevenTammen/stenotype](https://github.com/StevenTammen/stenotype)
**License:** GPL
**Category:** ELECTRICITY_MANAGEMENT
**Anticloud Integration:** PAX L5 Narrow L2 General 27B + AIOSS + Offline-First

## Upstream Description

(swap) Use: github.com/openwrt/openwrt — Smart router energy mgmt

## Anticloud Architectural Changes

1. PAX L5 Narrow L2 General 27B local load forecasting and fault prediction — edge deployment
2. AIOSS tamper-evident grid event log (NERC CIP aligned)
3. AES-256 encryption for all metering and SCADA data
4. Single-binary EMS deployment on utility substation hardware
5. Zero-cloud: all analytics and control logic run on local servers
6. GPU/CPU equalizer: real-time inference on edge GPU or CPU
7. Offline demand response optimization replacing cloud DR APIs
8. Open IEC 61968/61970 CIM integration replacing proprietary SCADA middleware

## Integration Points

- **PAX Inference Socket:** Local HTTP endpoint at `127.0.0.1:11434/v1/chat` — same OpenAI-compatible API, zero cloud
- **AIOSS Hook:** Every write operation calls `aioss_append(event, payload)` before commit
- **Encryption Layer:** All file I/O routed through `anticloud_crypto.encrypt_at_rest()`
- **Single Binary Build:** `pyinstaller anticloud_stenotype.spec` or `go build -o stenotype`

## Deployment Modes

| Mode | Hardware | Notes |
| --- | --- | --- |
| Edge CPU | Raspberry Pi 4 / Intel NUC | Full feature set, PAX on CPU |
| Desktop GPU | RTX 3060 / A10 | PAX GPU inference, <1s latency |
| Server | 2× A100 | Full batch throughput |
| Air-gapped | Any x86/ARM | Zero network dependency |