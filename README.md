# Intrusion Detection System (IDS)

A simple Python-based network intrusion detection system, plus a guide
for using the industry-standard tool Snort.

## What it does
**Python IDS (ids.py):**
- Sniffs live network traffic
- Alerts on traffic to suspicious ports (Telnet, RDP, SMB)
- Detects possible port scans (many ports hit by one IP in a short time)

**Snort guide (in the code comments at the bottom of ids.py):**
- How to install and run real Snort
- Example custom detection rules
- How rule syntax works

## Concepts covered
- Packet sniffing
- Signature-based detection
- Anomaly-based detection (port scan pattern)
- Industry IDS tools (Snort)

## Setup
```
pip install scapy
```

## Run
Sniffing requires elevated privileges:
```
sudo python3 ids.py
```
Press Ctrl+C to stop monitoring.

## ⚠️ Legal Note
Only monitor networks/traffic you own or have permission to monitor.
Packet sniffing on networks you don't control is illegal in most
countries.
