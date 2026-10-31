# ⚡ NetSuite: NetGuardian & NetFusion Studio

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-brightgreen.svg)]()
[![Release](https://img.shields.io/badge/Release-v1.0-orange.svg)](https://github.com/Bader287/netsuite/releases/tag/v1.0)
[![Website](https://img.shields.io/badge/Live_Site-GitHub_Pages-blueviolet.svg)](https://bader287.github.io/netsuite/)

> **A dual-engine desktop utility suite engineered for users constrained by ISP Fair Usage Policies (FUP), bandwidth throttles, and single-network Wi-Fi limits.**

🌐 **Live Download Website:** [https://bader287.github.io/netsuite/](https://bader287.github.io/netsuite/)

---

## 🚀 The Dual-Engine Architecture

NetSuite combines two dedicated applications designed to give you total control over your Internet connectivity:

```
                  ┌────────────────────────────────────────┐
                  │            NETSUITE v1.0               │
                  └──────────────────┬─────────────────────┘
                                     │
            ┌────────────────────────┴────────────────────────┐
            ▼                                                 ▼
┌───────────────────────────────┐         ┌─────────────────────────────────┐
│     🛡️ NetGuardian App         │         │     🎛️ NetFusion Studio         │
├───────────────────────────────┤         ├─────────────────────────────────┤
│ • Daily Bandwidth / FUP Quota │         │ • Multi-Wi-Fi Aggregator        │
│ • Per-App Wi-Fi Usage Audit   │         │ • Boost Mode (Bonding + Failover│
│ • Kernel-Level Auto-Pause     │         │ • Control Mode (Policy Routing) │
│ • Midnight Auto-Rollover      │         │ • 1-Click System Proxy Dispatch │
└───────────────────────────────┘         └─────────────────────────────────┘
```

---

## 🛡️ Engine 1: NetGuardian

Designed for capped ISP connections (e.g. 28 GB daily quota with 20 GB FUP slowdown thresholds).

- **Custom Quota & FUP Limits:** Visual dual-progress bars tracking normal quota and throttle threshold.
- **Kernel-Level Process Suspend/Resume:** Automatically freezes heavy background downloaders (Steam, Epic Games, Riot Client, Battle.net, Torrent clients) *without killing them or losing download progress*.
- **Per-App Wi-Fi Audit:** Real-time table displaying exact Megabytes consumed per background process.
- **Flicker-Free UI:** High-performance in-place numeric rendering with zero UI jitter.
- **Midnight Auto-Reset:** Data counters seamlessly reset daily at 00:00:00 local time.

---

## 🎛️ Engine 2: NetFusion Studio

Combines multiple network interfaces (e.g., Laptop Wi-Fi + Phone USB Tethering or USB Wi-Fi dongle) into a unified, high-speed connection.

- **⚡ Boost Mode (Channel Bonding):**
  - Distributes outgoing TCP/HTTP requests round-robin across all active network adapters.
  - Multiplies download throughput and provides **automatic failover** if one Wi-Fi drops.
- **🎛️ Control Mode (Granular Traffic Steering):**
  - Dedicates specific network adapters to specific types of traffic (e.g., Interface 1 for heavy downloads, Interface 2 exclusively for low-latency Discord/Zoom/Gaming).
- **TCP_NODELAY Real-Time Engine:**
  - 64 KB optimized stream buffers with Nagle's algorithm disabled to eliminate packet latency.
- **1-Click System Proxy Integration:**
  - Automatically configures Windows system proxy (WinINet broadcast) so all browsers and apps route through the aggregator instantly without requiring a restart.

---

## 📥 Downloads

| Platform | Format | Link |
| :--- | :--- | :--- |
| **Windows 10 / 11** | Standalone Executables (`.exe`) | [Download Windows Binaries (v1.0)](https://github.com/Bader287/netsuite/releases/latest/download/NetSuite_Windows_Binaries.zip) |
| **macOS & Linux** | Python Source Package | [Download Cross-Platform Package](https://bader287.github.io/netsuite/downloads/NetGuardian_Suite_v1.0.zip) |

---

## 💻 Quick Start Guide

### 🪟 Windows (Pre-compiled Executables)
1. Download `NetSuite_Windows_Binaries.zip` from [Releases](https://github.com/Bader287/netsuite/releases/latest).
2. Extract the archive.
3. Run `NetGuardian.exe` or `NetFusion.exe` directly (no Python or dependencies required).

### 🍎 macOS
```bash
# Extract the source package
unzip NetGuardian_Suite_v1.0.zip
cd NetGuardian_Suite_v1.0

# Install dependencies
pip3 install psutil customtkinter

# Run
python3 net_guardian_app.py
# or
python3 net_fusion_app.py
```

### 🐧 Linux (Ubuntu / Debian / Arch)
```bash
sudo apt update && sudo apt install python3-tk python3-pip
pip install psutil customtkinter

# Run
python3 net_guardian_app.py
# or
python3 net_fusion_app.py
```

---

## 🔒 Security & Privacy

- **100% Local Execution:** No telemetry, no cloud relays, no tracking. All proxy and monitoring operations run entirely on `127.0.0.1`.
- **Closed Source Windows Distribution:** Pre-compiled PyInstaller executables protect internal business logic for client-facing distributions.
- **Non-Destructive Freezing:** NetGuardian uses native OS kernel suspension (`psutil.Process.suspend()`) rather than terminating processes, ensuring safe resumption without corrupting game downloads.

---

## 📄 License

Distributed under the MIT License. See [LICENSE](LICENSE) for more information.
