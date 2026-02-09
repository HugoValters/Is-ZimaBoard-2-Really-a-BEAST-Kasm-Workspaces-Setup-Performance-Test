#  ZimaBoard 2 Ultimate Cyber Lab: Kasm Workspaces Setup (2026)

[![Status](https://img.shields.io/badge/Status-Tested%20%26%20Stable-success)]()
[![Hardware](https://img.shields.io/badge/Hardware-ZimaBoard%202-blue)]()
[![Software](https://img.shields.io/badge/Software-Kasm%20Workspaces%201.18-orange)]()
[![Category](https://img.shields.io/badge/Category-Cybersecurity%20%7C%20DevOps-red)]()

##  Overview

Turn your **ZimaBoard 2** into a fortress of privacy and a portable penetration testing lab using **Kasm Workspaces**.

This repository contains the full installation guide, configuration hacks, and performance benchmarks for running **Kali Linux**, **VS Code**, and **Tor Browser** inside isolated Docker containers. Unlike the original ZimaBoard, the new ZimaBoard 2 (4 Cores, 3.60 GHz) handles browser isolation with **ZERO LAG**.

###  [Watch the Full Step-by-Step Tutorial on YouTube](https://youtu.be/t1AprD1Kn5U)

---

##  Table of Contents
- [Hardware Requirements](#-hardware-requirements)
- [Installation Guide](#-installation-guide-5-minutes)
- [Pro Configuration Hacks](#-pro-configuration-hacks)
- [Stress Test Results](#-stress-test-results)
- [Final Verdict](#-final-verdict)

---

## ⚙️ Hardware Requirements

* **Device:** ZimaBoard 2 (Active Cooling recommended)
* **CPU:** 4 Cores, 3.60 GHz
* **OS:** Ubuntu / Debian / ZimaOS (Linux)
* **Storage:** SSD recommended for smooth container streaming.

---

## Installation Guide (5 Minutes)

We are installing **Kasm Workspaces 1.18.1**. In my tests, this process took exactly **5.5 minutes**.

Run these commands in your ZimaBoard terminal (SSH):

### 1. Navigate to Temp Directory
```bash
cd /tmp
```

### 2. Download Kasm
*Note: Always check the [official Kasm downloads](https://kasmweb.com) for the latest version.*
```bash
curl -O https://kasm-static-content.s3.amazonaws.com/kasm_release_1.18.1.d09dbc.tar.gz
```

### 3. Extract Archive
```bash
tar -xf kasm_release_1.18.1.d09dbc.tar.gz
```

### 4. Run Installer
```bash
sudo bash kasm_release/install.sh
```

> **IMPORTANT:** Once the installation finishes, the terminal will display your **Admin Login Credentials**. Save them immediately!

---

## Pro Configuration Hacks

Out of the box, Kasm sessions expire quickly. Use this hack to make your dev environment persistent.

### Extend Session Time Limit (Infinite Session)
1.  Log in to Kasm Web UI.
2.  Go to **Admin** -> **Settings**.
3.  Add a new setting named: `session_time_limit`.
4.  Set the value to: `999999` (this keeps it running for days).

### Persistent Data
* Use the "Disconnect" feature instead of "Delete" to resume your VS Code work later.

---

##  Stress Test Results

Is the ZimaBoard 2 actually a beast? I ran the following **simultaneously**:

1.  **Kali Linux** (Docker Container)
2.  **VS Code** (Remote Dev)
3.  **YouTube 1080p Playback** (Inside Firefox Container)

| Metric | Original ZimaBoard | ZimaBoard 2 |
| :--- | :--- | :--- |
| **Video Playback** | Choppy / Laggy | **Smooth (No Drops)** |
| **Multitasking** | Struggled | **Effortless** |
| **Fan Noise** | Silent (Passive) | **Whisper Quiet** |

---

## Final Verdict

If you are upgrading from a Raspberry Pi or the original ZimaBoard, the ZimaBoard 2 is a **massive upgrade**. The active cooling and 3.60 GHz clock speed make it a viable desktop replacement for self-hosting resource-heavy apps like Kasm.

**Pros:**
* ✅ Insane performance for the size.
* ✅ Easy 5-minute setup.
* ✅ 2.5GbE Networking.

**Cons:**
* Metal casing scratches easily (Handle with care!).

---

## Useful Links

* **Full Written Guide:** [Read on Medium](https://blog.valters.eu/turn-your-zimaboard-2-into-an-ultimate-cyber-lab-with-kasm-2026-guide-68a6f5075285)
* **Video Tutorial:** [Watch on YouTube](https://youtu.be/t1AprD1Kn5U)
* **KASM: :** [KASM Homepage](https://kasm.com)
* **Purchase ZIMA 2: :** [Zima store ]([https://kasm.com](https://bit.ly/3LPWV6Q) **( Discount coupon: ValtersTechTurf15 )**
* **Recommended Hosting:** [Zone.eu](https://www.zone.eu)

---

### Author

**Hugo Valters** *DevOps | Cybersecurity | HomeLab Enthusiast*

[![Medium](https://img.shields.io/badge/Medium-Follow-black?logo=medium)](https://blog.valters.eu)
[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-red?logo=youtube)](https://www.youtube.com/@hugovalters)
[![X](https://img.shields.io/badge/X-Follow-blue?logo=x)](https://x.com/hugovalters)

_Disclaimer: This project is for educational purposes only. Always use cybersecurity tools responsibly._
