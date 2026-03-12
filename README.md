# 💼 Upwork Projects Portfolio

> Freelance engineering projects completed in collaboration with **GenXI Tech Solutions** on Upwork.
> Covering PCB design, IoT systems, and vintage hardware schematic recreation.

---

## 📁 Projects Index

| # | Project | Domain | Status |
|---|---------|--------|--------|
| 1 | [🌿 Greenhouse Ventilation Control System](#-project-1--greenhouse-ventilation-control-system-pcb-design) | PCB / IoT / Embedded | ✅ Completed |
| 2 | [🎚️ Lexicon 224X Timing & Control Schematic](#%EF%B8%8F-project-2--lexicon-224x-timing--control-schematic-recreation) | Digital Electronics / Schematic | ✅ Completed |

---

---

## 🌿 Project 1 — Greenhouse Ventilation Control System PCB Design

### 📌 Overview

A complete **schematic and PCB design** for a greenhouse automation controller built for a client on Upwork. The system monitors environmental conditions inside a greenhouse and automatically controls ventilation to maintain optimal growing conditions.

Built around the **Particle Boron 404X** microcontroller, it communicates with **RuuviTag BLE wireless sensors** for real-time temperature and humidity data. All system data is streamed to the **Blynk IoT Platform** for remote cloud monitoring.

---

### ⚙️ System Functionality

| Component | Role |
|-----------|------|
| 🌀 **GAHT Fan** (Ground-to-Air Heat Transfer) | Circulates air through underground loop — regulates temperature, humidity & thermal stratification |
| 💨 **HAF Fan** (Horizontal Air Flow) | Maintains continuous horizontal air circulation — reduces disease risk from stagnant air |
| 📡 **RuuviTag BLE Sensors** | Wireless environmental monitoring (temperature & humidity) |
| ☁️ **Blynk IoT Platform** | Cloud dashboard for remote monitoring and control |

---

### 🧩 Hardware Architecture

```
Particle Boron 404X (MCU + Cloud)
        │
        ├── RuuviTag BLE Sensors  →  Temperature & Humidity
        ├── ACS712 Current Sensor →  Fan fault detection
        ├── Relay / Switch Circuit →  Fan control (GAHT & HAF)
        └── Blynk Cloud Dashboard →  Remote monitoring
```

---

### 🖨️ PCB Design Details

> **2-Layer PCB** designed following professional layout practices for reliability and manufacturability.

| Design Parameter | Value |
|-----------------|-------|
| Board Layers | 2-layer |
| Electrical Clearance | 3.2 mm between power domains |
| Signal Trace Width | 0.25 mm – 0.30 mm |
| Ground Plane | Solid pour with stitching vias |
| DRC Errors | **0** |
| DRC Warnings | **0** |
| Unconnected Nets | **0** |

**Key Layout Features:**
- ✅ Separation of high-voltage and low-voltage sections
- ✅ Solid ground plane for signal stability
- ✅ Ground stitching vias to reduce EMI
- ✅ Optimized component placement for enclosure fit

---

### ⚡ Fault Monitoring

An **ACS712 current sensing module** monitors fan current in real-time to detect:

- 🔴 Fan malfunction
- 🔴 Electrical faults
- 🔴 Overload conditions

Fault events are reported directly through the Blynk cloud dashboard.

---

### 📦 Manufacturing Outputs

- ✅ Gerber files
- ✅ Drill files
- ✅ Bill of Materials (BOM)
- ✅ DRC passed — 0 errors, 0 warnings, 0 unconnected nets

---

### 🛠️ Tools & Technologies

`KiCad` · `Particle Boron 404X` · `RuuviTag BLE` · `ACS712` · `Blynk IoT` · `PCB Layout` · `Gerber`

---

---

## 🎚️ Project 2 — Lexicon 224X Timing & Control Schematic Recreation

### 📌 Overview

A professional **schematic recreation** of the timing and control circuit from the **Lexicon 224X Digital Reverb System** — a legendary studio audio processor from the late twentieth century, widely respected in professional signal processing.

The goal was to digitally reconstruct the original hardware design using modern EDA tools while faithfully preserving the circuit architecture and logic of the historical design. The schematic was rebuilt from the final pages of original service documentation.

> Completed on Upwork in collaboration with **GenXI Tech Solutions**. Also served as a practical exercise in electrical engineering, digital electronics, and circuit analysis.

---

### 🧠 Design Challenges

Working with legacy hardware from an earlier generation of digital electronics presented unique challenges:

| Challenge | Approach |
|-----------|----------|
| 📄 Legacy service documentation | Carefully interpreted original schematics |
| 🔌 Obsolete ICs not in modern libraries | Manually recreated custom schematic symbols |
| 🔁 Correct signal flow preservation | Cross-referenced datasheets and service manuals |
| 📐 Modern schematic standards | Applied current EDA best practices throughout |

---

### 🔧 Custom Schematic Symbols Created

Because many legacy components are absent from standard libraries, the following custom symbols were designed from scratch:

| IC | Description |
|----|-------------|
| `AM8304N` | Digital audio processing IC — control logic |
| `MCM68B10` | RAM memory interface component |
| `74S112` | Dual JK flip-flop logic device |
| `74S00` | Quad NAND gate logic IC |
| `74S163 / 74LS163` | 4-bit synchronous binary counter |
| `74F374` | Octal edge-triggered flip-flop |

> All symbols recreated based on original datasheets for correct pin mapping and logical representation.

---

### 🔬 Circuit Section Recreated

The recreated schematic covers the **Timing & Control Section** of the Lexicon 224X, which coordinates internal digital operations including:

```
┌─────────────────────────────────────────────┐
│         TIMING & CONTROL SECTION            │
│                                             │
│  ┌──────────┐   ┌──────────┐   ┌─────────┐ │
│  │  Logic   │   │ Address  │   │ Memory  │ │
│  │  Gates & │──▶│ Counters │──▶│Interface│ │
│  │ Flip-Flops│   │          │   │         │ │
│  └──────────┘   └──────────┘   └─────────┘ │
│         │                                   │
│  ┌──────▼──────────────────────────────┐   │
│  │   Clock / Timing / Control Signals  │   │
│  └─────────────────────────────────────┘   │
└─────────────────────────────────────────────┘
```

**Includes:**
- ⏱️ Logic gates and flip-flops
- 🔢 Address counters
- 🧠 Memory interface connections
- 🕐 Clock and timing signals
- 🔀 Control signal routing

---

### 🎯 Purpose of the Recreation

| Goal | Value |
|------|-------|
| 📚 Modern documentation | Legacy hardware made accessible digitally |
| 🔍 Circuit analysis | Study of vintage digital audio systems |
| 🧪 Simulation readiness | Compatible with modern EDA tools |
| 🏛️ Historical preservation | Classic audio engineering design preserved |

---

### 🛠️ Tools & Technologies

`KiCad` · `Custom Symbol Design` · `Legacy IC Recreation` · `Digital Logic` · `Schematic Capture` · `Service Manual Analysis`

---

---

## 👤 About

| | |
|-|---|
| 👨‍💻 **Freelancer** | Amir Rehman |
| 🌐 **GitHub** | [@amirrehman19](https://github.com/amirrehman19) |
| 🤝 **Client** | GenXI Tech Solutions |
| 💼 **Platform** | Upwork |
| 📅 **Year** | 2026 |

---

> *These projects demonstrate the integration of embedded systems, PCB design, IoT connectivity, and digital electronics — from modern IoT agriculture solutions to preservation of classic audio hardware.*
