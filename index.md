# Self-Directed Technical Research & Lab Work
**Colton Lewis Davis**

Driven by a lifelong curiosity for how things work, I spend my personal time exploring the "full stack" of modern technology—from raw Electrical Theory and Radio Frequency to the software and security layers that sit on top of them.

---

### 🖥️🥼 Virtualization & Lab Architecture
Designed dedicated lab environments using **VMware** and **VirtualBox** to bridge the gap between theory and practice, with additional experience in **Hyper-V** integration. Includes the custom deployment of specialized **Kali Linux** or **Parrot OS** distributions and Windows target machines to study attack/defense scenarios.

### 📶🔐 Wireless Security & Hardware Interfacing
Utilizing specialized Wireless Network Adapters with **monitor mode** and **packet injection** capabilities to perform 802.11 stack analysis and network troubleshooting within a controlled lab environment.

### 📡⚙️ Radio Frequency (RF) Reverse-Engineering
Analyzing sub-GHz consumer devices to decode signals and study **rolling code encryption protocols**. Includes custom antenna design and optimization to improve signal-to-noise ratios.

### 📊✈️ Signal Analysis & Aviation Tracking
Operating **Software Defined Radio (SDR)** hardware for signal acquisition and spectrum analysis. Successfully deployed and hosted a local dump1090 aviation tracking server, managing real-time ADS-B data decoding and network distribution.

### 🐍💻 Software Development & Data Analysis
Leveraging **Visual Studio and Python** to analyze captured signal data. Focusing on the logic and structure of bitstreams to better understand cryptographic implementations at the hardware level.

### 📜🚀 Professional Development
* **CompTIA A+** (In Progress)
* **FCC Amateur Radio License** (Technician Class - In Progress)

# Project Objective: Mighty Mule RF Security & Optimization

## Phase I: Signal Integrity & RSSI Benchmarking
**Goal:** Comparative analysis of legacy vs. new transmitter output.
* **Analysis:** Benchmarking the output power (measured in dBFS) of legacy transmitters against new replacement units.
* **Controlled Variables:** All tests conducted with a standardized 3.0V DC power source (new batteries with voltage tested at 3.2v) and maintained at a fixed 1-meter distance from the receiver to ensure data consistency.
* **Metrics:** Establishing a baseline for Signal-to-Noise Ratio (SNR) and spectral purity to diagnose hardware degradation and intermittent range issues in aging units.

## Phase II: Signal Decoding & Cryptographic Assessment
**Goal:** Bitstream extraction and security audit.
* **Capture:** Utilizing SDR++ and Universal Radio Hacker (URH) to isolate the OOK (On-Off Keying) pulse-stream.
* **Objective:** Decoding the bitstream for Fixed-Code vs. Rolling-Code analysis. This determines the system's susceptibility to Replay Attacks and brute-force "fixed-bit" exploitation.



## Phase III: Receiver Hardware Optimization (Antenna Design)
**Goal:** Custom-tuned 1/4 Wave Monopole Implementation.
* **Design:** Engineering a custom-tuned antenna to replace the high-loss PCB-trace/press-on factory antenna.
* **Execution:**
    * Calculating optimal element length for the 318 MHz center frequency.
    * Implementing a dedicated ground plane to reduce SWR (Standing Wave Ratio).
    * Interfacing directly with the receiver PCB's RF input to minimize insertion loss.

---

### Technical Capture Specifications (SDR++)
| Setting | Value | Rationale |
| :--- | :--- | :--- |
| **Gain** | 0.9 dB | Prevents LNA saturation/clipping from proximity. |
| **AGC** | OFF | Maintains consistent amplitude for data analysis. |
| **Offset Tuning** | ENABLED | Shifts DC spike away from 318 MHz center. |
| **IQ Correction**| ENABLED | Eliminates spectral mirroring/ghost images. |
| **Radio Mode** | AM | Optimal for visualizing/hearing OOK pulse-width. |
| **Bandwidth** | 15.0 kHz | High SNR; isolates carrier from noise floor. |

---

### 🎥 Project Demonstration Videos Coming Soon......🛰️ [UPLINK] PENDING VIDEO UPLOAD...
* **[Build: dump1090 Aviation Server Deployment]** - *(Photos/Video Coming Soon)*
* **[Analysis: Decoding Mighty Mule Sub-GHz Gate Openers with SDR++]** - *(Photos/Video Coming Soon)*
* **[Wireless: 802.11 Network Mapping & Analysis using Kismet]** - *(Photos/Video Coming Soon)*
* **[Scripting: Python Bitstream Parser for Captured RF Data]** - *(Photos/Video Coming Soon)*
* **[Lab: Hardening Windows Target Machines against Kali Linux Exploits]** - *(Photos/Video Coming Soon)*
