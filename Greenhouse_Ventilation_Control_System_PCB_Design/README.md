# 🌿 Greenhouse Ventilation Control System
## PCB & Hardware Design

> 🌱 *Smart agriculture through embedded IoT — automated climate control for optimal greenhouse growing conditions.*

[![Platform](https://img.shields.io/badge/Platform-Upwork-14a800?style=flat-square&logo=upwork)](https://www.upwork.com)
[![Domain](https://img.shields.io/badge/Domain-PCB%20%26%20IoT%20Design-blue?style=flat-square)]()
[![MCU](https://img.shields.io/badge/MCU-Particle%20Boron%20404X-red?style=flat-square)]()
[![Cloud](https://img.shields.io/badge/Cloud-Blynk%20IoT-purple?style=flat-square)]()
[![Status](https://img.shields.io/badge/Status-Completed-success?style=flat-square)]()
[![Collaboration](https://img.shields.io/badge/In%20Collaboration%20With-GenXI%20Tech%20Solutions-orange?style=flat-square)](https://github.com/amirrehman19)

---

## 📌 Project Overview

This project involved the complete **schematic and PCB design** of a greenhouse automation controller developed for a client on **Upwork**. The system monitors real-time environmental conditions inside a greenhouse and automatically controls ventilation to maintain optimal growing conditions.

The controller is built around the **Particle Boron 404X** microcontroller, which communicates wirelessly with **RuuviTag BLE sensors** for live temperature and humidity data. All system data streams to the **Blynk IoT Platform**, enabling remote cloud-based monitoring and control.

> 🤝 *This project was completed in collaboration with **GenXI Tech Solutions**.*

---

## ⚙️ System Functionality

The system manages two ventilation mechanisms inside the greenhouse:

| Fan | Full Name | Role |
|-----|-----------|------|
| 🌀 **GAHT Fan** | Ground-to-Air Heat Transfer | Circulates air through an underground loop — regulates temperature, humidity & reduces thermal stratification |
| 💨 **HAF Fan** | Horizontal Air Flow | Maintains continuous horizontal air circulation — improves airflow & reduces plant disease risk |

The controller continuously processes sensor data and **automatically activates** these systems when environmental thresholds are reached.

---

## 🧩 Hardware Architecture

```
┌─────────────────────────────────────────────────────────┐
│              SYSTEM ARCHITECTURE                        │
│                                                         │
│   RuuviTag BLE Sensors                                  │
│   (Temp & Humidity) ──────┐                             │
│                           ▼                             │
│                  ┌─────────────────┐                    │
│                  │ Particle Boron  │──── Blynk IoT ☁️   │
│                  │     404X        │     Cloud Dashboard │
│                  └────────┬────────┘                    │
│                           │                             │
│              ┌────────────┴────────────┐                │
│              ▼                         ▼                │
│       ┌─────────────┐         ┌──────────────┐         │
│       │  GAHT Fan   │         │   HAF Fan    │         │
│       │  (Relay)    │         │   (Relay)    │         │
│       └─────────────┘         └──────────────┘         │
│                           │                             │
│                  ┌─────────────────┐                    │
│                  │ ACS712 Current  │                    │
│                  │    Sensor       │ ← Fault Detection  │
│                  └─────────────────┘                    │
└─────────────────────────────────────────────────────────┘
```

**Main Hardware Components:**

| Component | Role |
|-----------|------|
| 🧠 `Particle Boron 404X` | System control & cloud connectivity |
| 📡 `RuuviTag BLE Sensors` | Wireless temperature & humidity monitoring |
| ⚡ `ACS712 Current Sensor` | Fan current monitoring & fault detection |
| 🔌 `Relay / Switch Circuit` | Ventilation fan control |
| 🔋 `Power Supply & Protection` | Safe system operation |
| ☁️ `Blynk IoT Platform` | Remote cloud dashboard & monitoring |

---

## 🖨️ PCB Design Details

> **2-Layer PCB** designed following professional layout practices for reliability and manufacturability.

| Design Parameter | Specification |
|-----------------|---------------|
| 🗂️ Board Layers | 2-Layer |
| ⚡ Electrical Clearance | 3.2 mm between power domains |
| 📏 Signal Trace Width | 0.25 mm – 0.30 mm |
| 🔋 Power Traces | Wider traces for power distribution |
| 🌍 Ground Plane | Solid pour with stitching vias |
| ✅ DRC Errors | **0** |
| ✅ DRC Warnings | **0** |
| ✅ Unconnected Nets | **0** |

**Key Layout Features:**
- ✅ Separation of high-voltage and low-voltage sections
- ✅ 3.2 mm electrical clearance for safety between power domains
- ✅ Solid ground plane for improved signal stability
- ✅ Ground stitching vias to reduce EMI & noise
- ✅ Component placement optimized for enclosure fit

---

## ⚠️ Fault Monitoring

An **ACS712 current sensing module** monitors fan current in real-time to detect abnormal behavior:

| Fault Type | Indication |
|-----------|------------|
| 🔴 Fan Malfunction | Abnormal current draw detected |
| 🔴 Electrical Fault | Unexpected current spike or drop |
| 🔴 Overload Condition | Current exceeds safe threshold |

> Fault events are reported directly through the **Blynk cloud dashboard** for instant visibility.

---

## 📦 Manufacturing Outputs

Complete fabrication-ready outputs were generated:

- ✅ **Gerber Files** — Board layer data for fabrication
- ✅ **Drill Files** — Via and hole specifications
- ✅ **Bill of Materials (BOM)** — Full component list

> 🏆 Design passed **DRC with 0 errors, 0 warnings, and 0 unconnected nets** — fully ready for manufacturing.

---

## 🛠️ Tools & Technologies

`KiCad` &nbsp;·&nbsp; `Particle Boron 404X` &nbsp;·&nbsp; `RuuviTag BLE` &nbsp;·&nbsp; `ACS712` &nbsp;·&nbsp; `Blynk IoT` &nbsp;·&nbsp; `PCB Layout` &nbsp;·&nbsp; `Gerber Export` &nbsp;·&nbsp; `2-Layer PCB Design`

---

## ✅ Conclusion

This project demonstrates a practical application of **embedded systems and IoT in agriculture** — combining environmental sensing, automated ventilation control, and cloud monitoring into a reliable greenhouse climate management solution.

The design follows professional PCB layout standards ensuring **electrical safety**, **signal integrity**, and **manufacturing readiness**, while providing a scalable platform for future smart agriculture expansion.

> *"From soil to cloud — intelligent greenhouse automation through embedded IoT design."*

---

## 👤 About

| | |
|-|---|
| 👨‍💻 **Freelancer** | Amir Rehman |
| 🌐 **GitHub** | [@amirrehman19](https://github.com/amirrehman19) |
| 🤝 **Collaboration** | GenXI Tech Solutions |
| 💼 **Platform** | Upwork |
| 📅 **Year** | 2026 |

---

⬅️ *Back to [Upwork Projects Portfolio](../README.md)*
