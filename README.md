# Giant Company Open-Source Chip Design Summary

A curated summary of open-source chip design projects released by the world's leading IC design companies, highlighting their key value and application scenarios.

---

## 📊 Master Summary Table

> **Columns**: Project Name | Company | Category | Key Value | Application Scenarios | Star Rating

### 🔷 General-Purpose Processor Cores

| Project | Company | Category | Key Value | Application Scenarios |
|---------|---------|----------|-----------|----------------------|
| [A2O / A2I](https://github.com/openpower-cores/a2i) | **IBM** | CPU Core (POWER) | Out-of-order POWER processor core, multi-threaded (4-way SMT), up to 2.3 GHz | HPC, data center servers, cloud computing |
| [Microwatt](https://github.com/antonblanchard/microwatt) | **IBM** | CPU Core (POWER) | OpenPOWER soft-core in VHDL, small footprint FPGA implementation | Embedded systems, FPGA prototyping |
| [Nios V](https://www.intel.com/content/www/us/en/products/details/fpga/nios-processor/v.html) | **Intel** | CPU Core (RISC-V) | RISC-V soft processor for Intel FPGAs, RV32IA support | Embedded control, industrial IoT, automotive |
| [XuanTie (玄铁) Series](https://github.com/T-head-Semi) | **Alibaba T-Head** | CPU Core (RISC-V) | High-performance RISC-V cores (C906, C910 up to 2.5 GHz), Linux-capable | IoT, edge computing, AI inference, servers |
| [SweRV Cores](https://github.com/chipsalliance/Cores-SweRV) | **Western Digital** | CPU Core (RISC-V) | 2-way superscalar, 9-stage pipeline, up to 4.9 CoreMark/MHz | Storage controllers, embedded SoCs, IoT |

---

### 🔶 AI/ML Accelerators

| Project | Company | Category | Key Value | Application Scenarios |
|---------|---------|----------|-----------|----------------------|
| [NVDLA](https://github.com/nvdla/hw) | **NVIDIA** | Deep Learning Accelerator | Full open-source RTL for deep learning inference, scalable architecture (Small/Large) | Edge AI, autonomous vehicles, smart cameras, robotics |
| [CFU Playground](https://github.com/google/CFU-Playground) | **Google** | ML Accelerator Framework | Custom function unit design framework for ML on FPGAs, tightly coupled to RISC-V | Edge ML, TinyML, keyword spotting, gesture recognition |
| [XLS (Accelerator Synthesis)](https://github.com/google/xls) | **Google** | HLS Toolchain | High-level synthesis from C++/DSLX to Verilog, flexible accelerator design flow | Custom accelerator design, ASIC/FPGA data path |

---

### 🔷 SoC Platforms & Security

| Project | Company | Category | Key Value | Application Scenarios |
|---------|---------|----------|-----------|----------------------|
| [OpenTitan](https://github.com/lowRISC/opentitan) | **Google** (co-led) | Silicon Root of Trust | Industry-first open-source secure silicon RoT, hardware security module | Secure boot, TPM replacement, data center security, Chromebooks |
| [OpenPOWER](https://github.com/open-power) | **IBM** | ISA & Ecosystem | Open ISA with reference designs, hardware abstraction layer | High-end servers, heterogeneous computing, cloud |
| [OpenCAPI](https://github.com/opencapi) | **IBM** | Coherent Interface | Open high-bandwidth coherent bus interface (25 GT/s) | Accelerator-attached memory, heterogeneous system architecture |

---

### 🔶 FPGA & Development Platforms

| Project | Company | Category | Key Value | Application Scenarios |
|---------|---------|----------|-----------|----------------------|
| [Vitis Libraries](https://github.com/Xilinx/Vitis_Libraries) | **AMD / Xilinx** | FPGA Acceleration Library | Open-source HLS libraries for finance, ML, database acceleration | FinTech, quantitative trading, genomics, video processing |
| [PYNQ](https://github.com/Xilinx/PYNQ) | **AMD / Xilinx** | FPGA Framework | Python productivity for FPGA-based systems, Jupyter-based | Education, rapid FPGA prototyping, edge computing |
| [FuseSoC](https://github.com/olofk/fusesoc) | **Intel** (community) | IP Package Manager | Build and package management system for HDL designs | RTL IP reuse, CI/CD for hardware design |

---

## 🏢 Company-by-Company Breakdown

### 🌐 Google
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **OpenTitan** | Security SoC | Silicon root of trust co-developed with lowRISC, verified RTL | ⭐ Active |
| **CFU Playground** | ML on FPGA | Hardware/software co-design for custom ML accelerators | ⭐ Active |
| **XLS** | EDA Tool | High-level synthesis (C++/DSLX → Verilog) with formal verification | ⭐ Active |
| **SkyWater 130nm PDK** | Foundry PDK | Fully open 130nm process design kit, enabling open-source tapeouts | ⭐ Active |

---

### 🟢 NVIDIA
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **NVDLA** | AI Accelerator IP | Scalable deep learning accelerator, full RTL + verification suite | ⭐ Active |
| **CUDA Libs (open-gpu-kernel-modules)** | Driver/Kernel | Open GPU kernel modules for Linux (Turing+) | ⭐ Active |
| **NeMo Megatron** | AI Training | Large-scale training infrastructure (software, not chip design) | ⭐ Active |

---

### 🔵 IBM
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **A2O / A2I Core** | CPU Core | High-performance POWER ISA core, in-order & out-of-order variants | ⚡ Mature |
| **Microwatt** | CPU Core (FPGA) | Small POWER-compliant FPGA core (VHDL) | ⭐ Active |
| **OpenCAPI** | Interconnect | 25 GT/s coherent bus, open standard | ⚡ Mature |
| **OpenBMC** | BMC Firmware | Open-source Linux Foundation project for baseboard management | ⭐ Active |

---

### 🔷 Intel
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **Nios V** | RISC-V Soft CPU | Official RISC-V soft core for Intel FPGA platforms | ⭐ Active |
| **OPAE (Open Programmable Acceleration Engine)** | FPGA Framework | C++ library for Intel FPGA acceleration cards (PAC) | ⭐ Active |
| **oneAPI / DPC++** | Cross-architecture | Unified programming model for CPU/GPU/FPGA (software stack) | ⭐ Active |

---

### 🟠 AMD / Xilinx
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **Vitis Libraries** | FPGA Libraries | 400+ open-source HLS libraries for domain-specific acceleration | ⭐ Active |
| **PYNQ** | FPGA Framework | Jupyter-based Python framework for Xilinx SoCs | ⭐ Active |
| **Vitis AI** | AI Compiler | AI inference optimization for AMD/Xilinx platforms | ⭐ Active |
| **RapidWright** | FPGA Tools | Open-source FPGA CAD backend for custom place & route | ⭐ Active |

---

### 🟣 HUAWEI / HiSilicon
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **openEuler** | Server OS | Optimized for Kunpeng (ARM) & x86 servers, openEuler kernel | ⭐ Active |
| **openGauss** | Database | Enterprise-grade OLTP database optimized for ARM | ⭐ Active |
| **MindSpore** | AI Framework | Deep learning framework for Ascend NPU + GPU/CPU | ⭐ Active |
| **Kunpeng BoostKit** | Acceleration SDK | System-architecture acceleration kits for Kunpeng processors | ⭐ Active |

> **Note**: HUAWEI's open-source efforts focus on software ecosystem (OS, database, AI framework) around their chip hardware (Kunpeng, Ascend). Chip RTL is proprietary.

---

### ⚪ Samsung
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **Tizen** | OS | Open-source embedded OS for TVs, wearables | ⚡ Mature |
| **ONE (On-device Neural Engine)** | AI Inference | On-device AI runtime (software) | ⭐ Active |

> **Note**: Samsung has minimal open-source chip design RTL. Their major contributions are in software/SDK layers for Exynos/ISOCELL.

---

### 🔴 Qualcomm
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **Qualcomm AI Engine Direct SDK** | AI SDK | Direct AI acceleration on Snapdragon Hexagon | ⭐ Active |
| **FastCV** | Computer Vision | Mobile-optimized CV library for Snapdragon | ⚡ Mature |
| **RB5 Robotics Kit** | Robotics Platform | Qualcomm Robotics RB5 with open software tools | ⭐ Active |

> **Note**: Qualcomm's open-source focus is on SDKs and software stacks for Snapdragon SoCs. Core chip RTL remains proprietary.

---

### ⚫ MediaTek
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **LinkIt Platform** | IoT SDK | Hardware + software developer platform for IoT | 🟡 Archived |
| **Genio Platform** | IoT/Edge | Edge AI platform for smart displays, robotics | ⭐ Active |

> **Note**: MediaTek has minimal open-source chip design. Their open contributions are through the Linux/Android kernel community.

---

### 🟡 Apple
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **WebKit** | Browser Engine | Rendering engine for Safari, optimized for Apple Silicon | ⭐ Active |
| **Swift** | Programming Language | LLVM-based language optimized for Apple's hardware | ⭐ Active |
| **Core ML Stable Diffusion** | ML Models | Optimized Core ML models for Apple Neural Engine | ⭐ Active |

> **Note**: Apple does **not** release open-source chip design RTL. M-series, A-series, and U-series chip designs are fully proprietary.

---

### ⚪ Marvell
| Project | Category | Key Value | Status |
|---------|----------|-----------|--------|
| **OCTEON LiquiIO** | SmartNIC SDK | Software-defined data plane for OCTEON DPU | ⭐ Active |

> **Note**: Marvell has negligible open-source chip design. Their OCTEON and ThunderX data processing units are proprietary.

---

## 📈 Comparison: Open-Source Hardware Maturity by Company

```
Company         │ CPU Core │ AI Accel │ SoC Platform │ EDA Tools │ PDK/Foundry
─────────────────┼──────────┼──────────┼──────────────┼───────────┼────────────
Google           │    ○     │    ●     │      ●       │     ●     │     ●
NVIDIA           │    ○     │    ●     │      ○       │     ○     │     ○
IBM              │    ●     │    ○     │      ●       │     ○     │     ○
Intel            │    ◐     │    ○     │      ○       │     ◐     │     ○
AMD / Xilinx     │    ◐     │    ◐     │      ◐       │     ◐     │     ○
HUAWEI           │    ○     │    ○     │      ○       │     ○     │     ○
Samsung          │    ○     │    ○     │      ○       │     ○     │     ○
Qualcomm         │    ○     │    ○     │      ○       │     ○     │     ○
MediaTek         │    ○     │    ○     │      ○       │     ○     │     ○
Apple            │    ○     │    ○     │      ○       │     ○     │     ○
Marvell          │    ○     │    ○     │      ○       │     ○     │     ○
Alibaba T-Head   │    ●     │    ○     │      ○       │     ○     │     ○
Western Digital  │    ●     │    ○     │      ○       │     ○     │     ○
─────────────────┴──────────┴──────────┴──────────────┴───────────┴────────────
● = Significant open-source  ◐ = Partial/emerging  ○ = Minimal/none
```

---

## 🎯 Key Takeaways

1. **Google** leads in open-source chip design, with OpenTitan (silicon RoT), CFU Playground, and XLS covering security, ML, and EDA.
2. **NVIDIA** made waves by open-sourcing NVDLA, a production-grade deep learning accelerator IP.
3. **IBM** pioneered open-source CPU cores with OpenPOWER and A2O, enabling university-level processor research.
4. **Intel / AMD** focus on open FPGA tools and libraries, not processor RTL.
5. **RISC-V** is the primary ISA enabling open-source CPU cores from Alibaba (XuanTie), WD (SweRV), and many startups.
6. **Apple, Qualcomm, MediaTek, Marvell** essentially have **zero** open-source chip design — their contributions are limited to software SDKs.

---

## 🤝 Contributing

PRs welcome! If you know of open-source chip design projects from major IC companies that are missing here, please submit a pull request.

---

## 📄 License

This summary is [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) — public domain.
