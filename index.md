# Colton Lewis Davis

I am a technical investigator driven by a lifelong, obsessive passion for science and the mechanics of the physical world. I don't just "work" with technology; I live it. From the moment I could talk and ask "why" or "how", I’ve been driven to deconstruct how things work. Picture a 5-year-old with a spaghetti-stained mouth, screwdriver in hand, taking apart every household electronic in sight—that drive has never left me. 

My professional foundation is built on 11 years of manufacturing electromechanical devices. I am a builder who thrives in high-stakes, demanding environments. I like to look at the bigger picture and fully understand how systems work. Whether I’m at a lab bench or in the field, I approach every problem with the analytical mindset of a scientist. 

**Core Philosophy:**
I possess a radical drive to understand the underlying systems of our universe; I recognize the same patterns of logic in the predictable chaos of geological systems as I do during complex signal analysis. Whether it is a viral replication cycle in a microorganism or malware, I seek to understand how the system functions at its most fundamental level. For some reason however, after all these years, it seems like I only have more questions. I guess that innate curiosity is really what makes me, me. I hold a deep respect for the uncompromising rigor of pioneers like Marie Curie and Nikola Tesla and am committed to the betterment of mankind through disciplined research.

---

## Self-Directed Technical Research & Lab Work

### 📜🚀 Professional Development
* **CompTIA Security+** (In Progress)
* **FCC Amateur Radio License** (Technician Class - In Progress)

### 🖥️🥼 Virtualization & Lab Architecture
Designed dedicated lab environments using **VMware** and **VirtualBox** to bridge the gap between theory and practice, with additional experience in **Hyper-V** integration. Includes the custom deployment of specialized **Kali Linux** or **Parrot OS** distributions and Windows target machines to study attack/defense scenarios.

### 📶🔐 Wireless Security & Hardware Interfacing
Utilizing specialized Wireless Network Adapters with **monitor mode** and **packet injection** capabilities to perform 802.11 stack analysis and network troubleshooting within a controlled lab environment.

### 📡⚙️ Radio Frequency (RF) Reverse-Engineering
Analyzing sub-GHz consumer devices to decode signals and study **rolling code encryption protocols**. Includes custom antenna design and optimization to improve signal-to-noise ratios.

### 📊✈️ Signal Analysis & Aviation Tracking
Operating **Software Defined Radio (SDR)** hardware for signal acquisition and spectrum analysis. Successfully deployed and hosted a local dump1090 aviation tracking server, managing real-time ADS-B data decoding and network distribution.



---

# Project Objective: Mighty Mule RF Security & Optimization

## Phase I: Signal Integrity & RSSI Benchmarking
**Goal:** Comparative analysis of legacy vs. new transmitter output.

**Analysis:** Benchmarking the output power (measured in dBFS) of legacy transmitters against new replacement units.

**Controlled Variables:** All tests conducted with a standardized **3V Lithium Coin Cell** (verified at 3.2V) and maintained at a fixed 1-meter distance from the receiver to ensure data consistency.

**Metrics:** Establishing a baseline for Signal-to-Noise Ratio (SNR) and spectral purity to diagnose hardware degradation.

### Technical Capture Specifications (SDR++)
| Setting | Value | Rationale |
| :--- | :--- | :--- |
| **Gain** | 0.0 dB | High-proximity capture; ensures zero LNA clipping for bitstream purity. |
| **AGC** | OFF | Maintains consistent amplitude for data analysis. |
| **Offset Tuning** | ENABLED | Shifts DC spike away from 318 MHz center. |
| **IQ Correction**| ENABLED | Eliminates spectral mirroring/ghost images. |
| **Radio Mode** | AM | Optimal for visualizing/hearing OOK pulse-width. |
| **Bandwidth** | 15.0 kHz | High SNR; isolates carrier from noise floor. |


<video width="100%" height="auto" controls>
  <source src="assets/videos/MightyMuleV2SignalTest1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

*Final Documentation and the rest of the video demonstrations are currently in post-production.*

---

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

### 🎥 Project Demonstration Videos
* **[Analysis: Decoding Mighty Mule Sub-GHz Gate Openers with SDR++]** - *(Video coming soon)*
* **[Build: dump1090 Aviation Server Deployment]** - *(Photos/Video Coming Soon)*
* **[Wireless: 802.11 Network Mapping & Analysis using Kismet]** - *(Photos/Video Coming Soon)*
* **[Scripting: Python Bitstream Parser for Captured RF Data]** - *(Photos/Video Coming Soon)*
* **[Lab: Hardening Windows Target Machines against Kali Linux Exploits]** - *(Photos/Video Coming Soon)*
