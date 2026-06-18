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

> HUAWEI hosts the largest chip ecosystem open-source portfolio among IC companies. All projects are on **[AtomGit/GitCode](https://atomgit.com)** (China's largest open-source forge) and some mirror on GitHub. While chip RTL remains proprietary, the surrounding software ecosystem is extensively open-sourced.

#### 🖥️ Kunpeng (鲲鹏) ARM Server Chip Ecosystem

| Project | AtomGit URL | Key Value | Status |
|---------|------------|-----------|--------|
| **openEuler** | [atomgit.com/openeuler](https://atomgit.com/openeuler) | Enterprise-grade Linux OS optimized for Kunpeng & multi-arch (ARM/x86/RISC-V), 825+ repos, 3.3K stars | ⭐ Active |
| **openEuler Kernel** | [atomgit.com/openeuler/kernel](https://atomgit.com/openeuler/kernel) | Kunpeng-optimized Linux kernel with NUMA, scheduler, and power management enhancements | ⭐ Active |
| **BishengJDK** | [atomgit.com/openeuler/bishengjdk-8](https://atomgit.com/openeuler/bishengjdk-8) | High-performance OpenJDK distribution optimized for Kunpeng ARM architecture | ⭐ Active |
| **Bisheng Compiler** | [atomgit.com/openeuler](https://atomgit.com/openeuler) | LLVM/GCC-based compiler toolchain with Kunpeng-specific optimizations (auto-vectorization, SVE) | ⭐ Active |
| **Kunpeng BoostKit** | [huaweicloud.com/kunpeng](https://www.huaweicloud.com/intl/zh-cn/solution/kunpeng/index.html) | System-level acceleration SDK: crypto, compression, DPDK, math libraries leveraging Kunpeng HW engines | ⭐ Active |
| **KAE (Kunpeng Accelerator Engine)** | [atomgit.com/openeuler/KAE](https://atomgit.com/openeuler) | HardWare offload APIs for Kunpeng's built-in crypto (RSA/ECDH/SMx) and compression (gzip/lz4) accelerators | ⭐ Active |
| **iSulad** | [atomgit.com/openeuler/iSulad](https://atomgit.com/openeuler/iSulad) | Lightweight container runtime (iSula) designed for cloud/edge Kunpeng deployments, OCI-compatible | ⭐ Active |
| **StratoVirt** | [atomgit.com/openeuler/stratovirt](https://atomgit.com/openeuler/stratovirt) | Rust-based lightweight VMM for Kunpeng servers, minimal attack surface | ⭐ Active |
| **A-Tune** | [atomgit.com/openeuler/A-Tune](https://atomgit.com/openeuler/A-Tune) | AI-powered OS auto-tuning engine for Kunpeng, optimizes 10+ subsystems automatically | ⭐ Active |
| **openLooKeng** | [atomgit.com/openLooKeng](https://atomgit.com/openLooKeng) | High-performance distributed SQL query engine for big data on Kunpeng | ⭐ Active |
| **openGauss** | [atomgit.com/opengauss](https://atomgit.com/opengauss) | Enterprise relational database, deeply optimized for Kunpeng multi-core ARM architecture (NUMA-aware) | ⭐ Active |
| **secGear** | [atomgit.com/openeuler/secGear](https://atomgit.com/openeuler) | Confidential computing SDK for Kunpeng TrustZone/TEE, framework for enclave development | ⭐ Active |
| **UMDK (Unified Memory Dev Kit)** | [atomgit.com/openeuler/umdk](https://atomgit.com/openeuler/umdk) | Memory-semantic networking stack for Kunpeng-based high-performance distributed systems | ⭐ Active |
| **karmada** | [atomgit.com/karmada](https://atomgit.com/karmada) | Open multi-cloud management platform (CNCF sandbox) for Kunpeng cloud infrastructure | ⭐ Active |

#### 🧠 Ascend (昇腾) AI NPU Ecosystem

| Project | AtomGit URL | Key Value | Status |
|---------|------------|-----------|--------|
| **MindSpore** | [atomgit.com/mindspore](https://atomgit.com/mindspore) | Deep learning framework with native Ascend NPU support, auto-parallel, auto-diff, 1K+ stars | ⭐ Active |
| **CANN (Compute Architecture for Neural Networks)** | [huawei.com/ascend](https://www.hiascend.com/) | Ascend operator library and compiler (AscendCL, TBE), exposing NPU compute to frameworks | ⭐ Active |
| **MindSpore Lite** | [atomgit.com/mindspore/mindspore-lite](https://atomgit.com/mindspore/mindspore-lite) | Lightweight on-device AI inference engine for Ascend edge NPU | ⭐ Active |
| **MindFormers** | [atomgit.com/mindspore/mindformers](https://atomgit.com/mindspore/mindformers) | LLM training/inference toolkit with Ascend-optimized distributed parallelism | ⭐ Active |
| **MindQuantum** | [atomgit.com/mindspore/mindquantum](https://atomgit.com/mindspore/mindquantum) | Quantum computing framework leveraging Ascend for simulation acceleration | ⭐ Active |
| **AKG (Auto Kernel Generator)** | [atomgit.com/mindspore/akg](https://atomgit.com/mindspore/akg) | TVM-inspired auto-scheduling operator generator for Ascend/GPU | ⭐ Active |
| **Hyper-Parallel** | [atomgit.com/mindspore/hyper-parallel](https://atomgit.com/mindspore/hyper-parallel) | Ascend superpod distributed parallelism library with topology-aware scheduling & FP8 training | ⭐ Active |
| **DVM** | [atomgit.com/mindspore/dvm](https://atomgit.com/mindspore/dvm) | Microsecond-level real-time AI operator compilation engine for dynamic shapes on Ascend | ⭐ Active |

#### 📱 HarmonyOS / IoT Open Chip Ecosystem

| Project | AtomGit URL | Key Value | Status |
|---------|------------|-----------|--------|
| **OpenHarmony** | [atomgit.com/openharmony](https://atomgit.com/openharmony) | Unified OS for IoT/embedded devices, runs on Kirin/Kunpeng and 100+ chip platforms | ⭐ Active |
| **Huawei LiteOS** | [atomgit.com/LiteOS](https://atomgit.com/LiteOS) | Lightweight real-time IoT OS, ported to Cortex-M, RISC-V, and HiSilicon IoT chips | ⚡ Mature |
| **Oniro (OpenAtom)** | [oniroproject.org](https://oniroproject.org/) | Eclipse Foundation multi-kernel OS (Zephyr + Linux), Huawei-contributed, multi-chip platform | ⭐ Active |

> **Key insight**: HUAWEI is the **only** company in this survey that runs its entire chip software stack (OS → database → AI framework → accelerators → security) on its own open-source forge (AtomGit/GitCode). No other chip giant has matched this ecosystem-wide open-source play. However, **chip RTL/design files remain proprietary** — the openness is at the software ecosystem layer surrounding the silicon.

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
HUAWEI           │    ◐     │    ◐     │      ◐       │     ◐     │     ○
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
7. **HUAWEI** is unique in open-sourcing its entire chip **software ecosystem** (OS → DB → AI → security) on its own forge (AtomGit), but keeps chip RTL proprietary.

---

## 💰 Open-Source Chip Design: Commercial Gain Principles

Why do giant IC companies with trillion-dollar valuations open-source their chip designs? The answer is never altruism — it's strategic business logic.

### 🧩 Strategy 1: Commoditize Your Complement

The most powerful economic principle in open-source hardware. A chip is never sold alone — it requires an ecosystem of software, tools, middleware, and developers to thrive.

| Company | Opens Source… | To Sell… | Mechanism |
|---------|--------------|----------|-----------|
| **HUAWEI** | openEuler, MindSpore, openGauss, KAE, CANN | Kunpeng servers, Ascend NPU cloud services, Kirin SoCs | Free OS + AI framework locks developers into Kunpeng/Ascend hardware, which requires paid Huawei Cloud or on-prem servers |
| **NVIDIA** | NVDLA accelerator IP | Data center GPUs, CUDA ecosystem, DGX systems | Free NVDLA IP trains engineers familiar with NVIDIA's inference architecture. Production-scale workloads require paid NVIDIA GPUs + CUDA |
| **Google** | OpenTitan, SkyWater PDK | Google Cloud, Titan security chips, Chromebooks | Open-sourcing silicon RoT creates de-facto security standard, reducing Google's own chip NRE costs through community validation |
| **Intel** | Nios V, OPAE FPGA libs | Xeon CPUs, Agilex FPGAs, foundry services | Free soft cores + FPGA tools expand the FPGA market, which drives demand for Intel's high-margin FPGA silicon |
| **AMD / Xilinx** | Vitis Libraries, PYNQ, RapidWright | Versal ACAPs, Alveo cards, FPGA silicon | Free libraries lower barrier to FPGA adoption. Each FPGA developer eventually needs to buy hardware |

### 🌐 Strategy 2: Set the Industry Standard

When a company open-sources their interface, protocol, or architecture, they're betting it becomes the industry default — and their proprietary ecosystem benefits.

| Company | Open Standard | Strategic Goal |
|---------|--------------|----------------|
| **IBM** | OpenPOWER ISA + OpenCAPI | Create a viable alternative to x86, driving POWER server sales and IBM Cloud/consulting |
| **Google** | OpenTitan RoT architecture | Establish an open security standard that reduces Google's per-device chip costs and makes Chrome OS/Android more secure |
| **NVIDIA** | NVDLA architecture + NVLink (partial) | Cement the data-flow accelerator paradigm as the industry norm for edge AI |

### 👨‍🔬 Strategy 3: Talent Cultivation & Academic Capture

Open-source chip designs are the ultimate university recruiting tool. Students trained on your architecture become your future hires — or at minimum, your future customers.

- **IBM**'s OpenPOWER/A2O cores are used in university computer architecture courses worldwide → graduates are fluent in POWER ISA
- **Google**'s CFU Playground is designed for ML hardware education → familiarizes next-gen engineers with Google's ML accelerator design patterns
- **NVIDIA**'s NVDLA is used in academic research on neural network accelerators → theses and papers reference NVIDIA architecture as baseline
- **HUAWEI**'s openEuler/MindSpore are taught in Chinese universities via "Smart Base" (智能基座) program → 700+ universities, 200K+ students trained on Kunpeng/Ascend stack

### 🔒 Strategy 4: Preempt Regulation & Build Trust

For security-critical chips (TPM, secure enclave, root of trust), closed-source designs face regulatory skepticism. Open-sourcing builds trust.

- **Google** open-sourced OpenTitan to prove its Titan chip has no backdoors, critical for government/enterprise procurement
- **HUAWEI** open-sources its entire software stack on AtomGit to address "trusted supply chain" requirements from Chinese government and SOEs
- **IBM** open-sources OpenBMC for server management transparency

### 📉 Strategy 5: Reduce NRE Costs Through Community Labor

Chip design is astronomically expensive. Open-sourcing non-differentiating IP crowdsources maintenance and verification.

| Company | Open-Sourced Component | Community Contributes |
|---------|----------------------|----------------------|
| **NVIDIA** | NVDLA RTL + verification suite | Bug fixes, new feature additions, tool integrations |
| **Google** | OpenTitan RTL + DV | Formal verification, FPGA testing, documentation |
| **Western Digital** | SweRV RTL | ASIC/FPGA porting, compiler optimization |
| **Alibaba** | XuanTie RTL | Ecosystem tools, Linux ports, application libraries |

### 🏭 Strategy 6: Drive Foundry Volume

More open-source tapeouts = more wafers through the fab. This is especially relevant for Google's SkyWater partnership.

- **Google + SkyWater + Efabless**: Free 130nm MPW shuttle → thousands of open-source designs fabricated → SkyWater gets volume, Google gets ecosystem
- **TSMC + open-source RISC-V**: More RISC-V tapeouts mean more N5/N3 wafers for TSMC's advanced nodes

### 🎯 The Golden Rule

> **"Open-source the ecosystem, sell the hardware. Open-source the infrastructure, sell the service. Open-source yesterday's innovation, sell tomorrow's."**

Companies that understand this rule — Google, NVIDIA, IBM, HUAWEI — thrive with open-source. Those that don't — Apple, Qualcomm — leave the open chip design space entirely to others.

### 📊 Commercial Motivation Matrix

```
                    Open-Sources to…
Company     │ Sell HW │ Set Std │ Talent │ Trust │ Cut Cost │ Drive Fabs
─────────────┼─────────┼─────────┼────────┼───────┼──────────┼───────────
HUAWEI       │    ●    │    ●    │   ●    │   ●   │    ◐     │    ○
Google       │    ●    │    ●    │   ●    │   ●   │    ◐     │    ●
NVIDIA       │    ●    │    ●    │   ◐    │   ○   │    ●     │    ○
IBM          │    ●    │    ●    │   ●    │   ◐   │    ●     │    ○
Intel        │    ●    │    ○    │   ◐    │   ○   │    ○     │    ○
AMD/Xilinx   │    ●    │    ◐    │   ◐    │   ○   │    ○     │    ○
Alibaba T-H  │    ●    │    ●    │   ◐    │   ○   │    ●     │    ○
WD           │    ◐    │    ○    │   ○    │   ○   │    ●     │    ○
─────────────┴─────────┴─────────┴────────┴───────┴──────────┴───────────
● Primary motive   ◐ Secondary motive   ○ Not applicable
```

---

## 🤝 Contributing

PRs welcome! If you know of open-source chip design projects from major IC companies that are missing here, please submit a pull request.

---

## 📄 License

This summary is [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) — public domain.
