# 🎚️ Lexicon 224X Digital Reverb
## Timing & Control Circuit — Schematic Recreation

> 🏛️ *Preserving a legend of studio audio engineering through modern schematic design.*

![Platform](https://img.shields.io/badge/Platform-Upwork-14a800?style=flat-square&logo=upwork)
![Domain](https://img.shields.io/badge/Domain-Digital%20Electronics-blue?style=flat-square)
![Type](https://img.shields.io/badge/Type-Schematic%20Recreation-purple?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-success?style=flat-square)
![collaborate](https://img.shields.io/badge/Client-GenXI%20Tech%20Solutions-orange?style=flat-square)

---

## 📌 Project Overview

This project involved the **digital reconstruction** of the timing and control schematic from the **Lexicon 224X Digital Reverb System** — a legendary professional audio processor widely used in studio signal processing during the late twentieth century.

The schematic was carefully rebuilt from the final pages of the original service documentation using modern EDA tools, preserving the original circuit architecture and logic with full fidelity.

> Completed as a freelance project on **Upwork** in collaboration with **GenXI Tech Solutions**.
> Also served as a practical deep-dive into electrical engineering, digital electronics, and circuit analysis.

---

## ⚠️ Design Challenges

The Lexicon 224X originates from an **earlier generation of digital electronics** — many of its ICs are completely absent from modern schematic libraries, requiring significant reverse-engineering effort.

| # | Challenge | Approach |
|---|-----------|----------|
| 1 | 📄 Interpreting legacy service documentation | Cross-referenced original service manuals carefully |
| 2 | 🔌 Mapping obsolete ICs to modern representations | Manually recreated missing components from datasheets |
| 3 | 🔁 Maintaining correct signal flow & logic relationships | Verified against original circuit topology |
| 4 | 🧩 Rebuilding missing library components | Designed custom symbols from scratch |
| 5 | 📐 Following modern schematic standards | Applied current EDA best practices throughout |

---

## 🔧 Custom Schematic Symbols Created

Because many legacy components were absent from standard libraries, the following **custom symbols** were designed from scratch based on original datasheets and service manual documentation:

| Symbol | Component | Description |
|--------|-----------|-------------|
| `AM8304N` | Digital Audio IC | Audio processing IC used in control logic |
| `MCM68B10` | RAM Interface | Memory interface component |
| `74S112` | Flip-Flop | Dual JK flip-flop logic device |
| `74S00` | Logic Gate | Quad NAND gate IC |
| `74S163 / 74LS163` | Counter | 4-bit synchronous binary counter |
| `74F374` | Flip-Flop | Octal edge-triggered flip-flop |

> ✅ All symbols recreated with correct pin mapping and logical representation for simulation compatibility.

---

## 🔬 Circuit Section Recreated

The recreated schematic covers the **Timing & Control Section** — the digital backbone that coordinates all internal operations of the reverb processor.

```
┌──────────────────────────────────────────────────────┐
│              TIMING & CONTROL SECTION                │
│                                                      │
│   ┌─────────────┐     ┌──────────────┐              │
│   │ Logic Gates │────▶│   Address    │              │
│   │ & Flip-Flops│     │   Counters   │              │
│   └─────────────┘     └──────┬───────┘              │
│                              │                       │
│                    ┌─────────▼────────┐              │
│                    │  Memory Interface│              │
│                    │   Connections    │              │
│                    └─────────┬────────┘              │
│                              │                       │
│          ┌───────────────────▼──────────────────┐   │
│          │   Clock · Timing · Control Signals   │   │
│          └──────────────────────────────────────┘   │
└──────────────────────────────────────────────────────┘
```

**This section includes:**

- ⏱️ **Logic gates and flip-flops** — combinational and sequential logic
- 🔢 **Address counters** — data addressing and sequencing
- 🧠 **Memory interface connections** — RAM coordination
- 🕐 **Clock and timing signals** — synchronization throughout the system
- 🔀 **Control signal routing** — orchestration of all subsystems

Together these elements regulate **data flow**, **synchronization**, and **address generation** within the processor's DSP architecture.

---

## 🎯 Purpose of the Recreation

| Goal | Value Delivered |
|------|----------------|
| 📚 Modern documentation | Legacy hardware made permanently accessible |
| 🔍 Circuit analysis | Deep study of vintage digital audio design |
| 🧪 Simulation readiness | Fully compatible with modern EDA tools |
| 🏛️ Historical preservation | Classic audio engineering architecture preserved |
| 🎓 Educational exploration | Usable reference for digital electronics study |

---

## 🛠️ Tools & Technologies

`KiCad` &nbsp;·&nbsp; `Custom Symbol Design` &nbsp;·&nbsp; `Legacy IC Recreation` &nbsp;·&nbsp; `Digital Logic Analysis` &nbsp;·&nbsp; `Schematic Capture` &nbsp;·&nbsp; `Service Manual Interpretation`

---

## ✅ Conclusion

Recreating this circuit required **careful interpretation of historical documentation** and the reconstruction of obsolete components within a modern design environment.

This project bridges **vintage digital audio technology** with modern schematic design practices — allowing the architecture of a historically important piece of studio hardware to remain accessible for study, simulation, and preservation.

> *"Classic audio engineering, reimagined for the modern era."*

---

## 👤 About

| | |
|-|---|
| 👨‍💻 **Freelancer** | Amir Rehman |
| 🌐 **GitHub** | [@amirrehman19](https://github.com/amirrehman19) |
| 🤝 **collaborate** | GenXI Tech Solutions |
| 💼 **Platform** | Upwork |
| 📅 **Year** | 2026 |

---

⬅️ *Back to [Upwork Projects Portfolio](../README.md)*
