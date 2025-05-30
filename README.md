# 🔍 digital-forensics-case-studies

This repository contains simulated case studies and investigations covering endpoint, memory, filesystem, and network-based digital forensics. Each folder is a step-by-step walkthrough of how artifacts were identified, timelines were built, and conclusions were drawn — using real tools and forensic logic.

## 🎯 Why This Repo?

You don’t truly understand an attack until you’ve **walked it back**:
- What ran?
- When?
- As who?
- From where?
- With what effect?

This repo builds that muscle by simulating post-compromise forensic investigations across multiple vectors.

## 🗂 What’s Included

| Folder | Focus |
|--------|-------|
| `endpoint-analysis/` | Artifact trails on Windows and Linux machines |
| `memory-analysis/` | Volatile memory captures using tools like Volatility |
| `file-system-analysis/` | NTFS/MFT, timestamp forensics, deleted file recovery |
| `network-forensics/` | PCAP-based cases, DNS tunneling, C2 patterns |
| `incident-timelines/` | End-to-end walkbacks of simulated incidents |
| `tooling-and-methodology/` | Tools, cheat sheets, custody templates |
| `docs/` | Templates and terminology to keep case studies consistent |

## 🧪 Sample Case: Linux Crontab Malware

- **Initial Clue**: High CPU usage and suspicious outbound DNS queries  
- **Findings**: Malicious script persisted via root crontab  
- **Artifacts**:  
  - `/etc/crontab` backdoor  
  - `/tmp/.dbus/` executable  
  - Bash history cleared  
- **Lessons**: Importance of crontab auditing and `/tmp` hardening

## 🧠 Ideal For

- Students prepping for GCFA, OSCP, or forensic analyst roles
- Blue teamers brushing up on artifact interpretation
- Anyone building incident response muscle memory
- Engineers shifting left into DFIR from sysadmin or netsec roles

## 🛠 Tooling Covered

- Volatility
- Autopsy
- Sleuth Kit
- Wireshark + TShark
- Linux CLI (strings, grep, lsof, find, stat)
- Windows tools (FTK Imager, Sysinternals, Event Viewer)
