# ⚡ NetFusion Max (v2.0 Unified Edition)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-brightgreen.svg)]()
[![Release](https://img.shields.io/badge/Release-v2.0-orange.svg)](https://github.com/Bader287/netsuite/releases/tag/v2.0)
[![Website](https://img.shields.io/badge/Live_Site-Vercel-black.svg)](https://netsuite-one.vercel.app)

> **All-in-One Multi-Wi-Fi Aggregator & Bandwidth FUP Guardian.**  
> Track per-Wi-Fi data spend, prevent ISP FUP slowdowns, bond multiple network adapters into one strong connection, and freeze heavy background apps with zero progress loss.

🌐 **Live Download Website:** [https://netsuite-one.vercel.app](https://netsuite-one.vercel.app)

---

## 🚀 Unified Architecture

NetFusion Max merges **NetGuardian** and **NetFusion** into a unified, dark-mode command center:

```
┌────────────────────────────────────────────────────────────────────────┐
│                   ⚡ NETFUSION MAX (v2.0 UNIFIED)                      │
├────────────────────────────────────────────────────────────────────────┤
│ 📡 Multi-Wi-Fi & FUP Monitor │ 🚀 Channel Bonding │ 📊 Per-App Audit   │
├──────────────────────────────┼────────────────────┼────────────────────┤
│ • Per-Adapter Data Spent (GB)│ • Boost Mode (RR)  │ • Per-App Usage MB │
│ • Dual Progress (Cap & FUP)  │ • Control Mode     │ • Interface Used   │
│ • Live Upload / Download Spd │ • 1-Click Proxy    │ • Kernel Freezing  │
│ • Latency / Health Watchdog  │ • Auto-Failover    │ • Auto-Pause Rules │
└──────────────────────────────┴────────────────────┴────────────────────┘
```

---

## ✨ Key Features

1. **📡 Individual Per-Wi-Fi FUP & Quota Tracking**
   - Independent dual progress bars for each detected Wi-Fi adapter or mobile hotspot.
   - Live speed (KB/s or MB/s), daily usage, and ping latency per adapter.
   - Customizable daily caps and FUP warning thresholds for every connection.

2. **🚀 Multi-Wi-Fi Bonding & Traffic Steering**
   - **Boost Mode (Channel Bonding):** Merges available Wi-Fi streams round-robin for combined throughput and seamless failover.
   - **Control Mode (Traffic Steering):** Steers heavy downloads to Wi-Fi 1, while dedicating low-latency Wi-Fi 2 to Discord, Zoom, and Games.
   - **1-Click System Proxy:** Routes all Windows network traffic through the bonded engine with instant WinINet broadcast notification.

3. **📊 Per-App Network Audit & Safe Freezing**
   - Live table of running network processes showing data consumed today and which adapter they use.
   - Non-destructive kernel suspension (`psutil.Process.suspend()`) to freeze heavy apps (Steam, Epic, Riot, Torrents) with zero download progress loss.
   - Automatic freeze trigger when approaching FUP slowdown limits.

---

## 📥 Downloads

| Platform | Format | Link |
| :--- | :--- | :--- |
| **Windows 10 / 11** | Standalone Executable (`.exe`) | [Download NetFusionMax Windows v2.0](https://github.com/Bader287/netsuite/releases/download/v2.0/NetFusionMax_Windows_v2.0.zip) |
| **macOS & Linux** | Python Cross-Platform Source | [Download Cross-Platform Package](https://netsuite-one.vercel.app/downloads/NetFusionMax_CrossPlatform_v2.0.zip) |

---

## 💻 Quick Start Guide

### 🪟 Windows (Pre-compiled Executable)
1. Download `NetFusionMax_Windows_v2.0.zip`.
2. Extract and run **`NetFusionMax.exe`** directly (no Python or dependencies required).

### 🍎 macOS / 🐧 Linux
```bash
unzip NetFusionMax_CrossPlatform_v2.0.zip
pip install psutil customtkinter
python3 netfusion_max_app.py
```

---

## 🔒 Full Security & Privacy Guarantee

- **100% Offline-First:** Runs exclusively on `127.0.0.1`. No telemetry, external servers, or tracking.
- **Code Protected:** Distributed as pre-compiled standalone binary on Windows so end users cannot view or alter internal source code.
- **Atomic State Persistence:** All data writes use atomic file replacement to prevent data corruption during sudden shutdowns.

---

## 📄 License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.
