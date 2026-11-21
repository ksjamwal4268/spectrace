# ⚡ SpecTrace — Autonomous Hardware Telemetry & ONDC Repair Protocol

> **Zero-install browser diagnostics for ₹0 warranty claims and 15-minute ONDC repairs.**

SpecTrace is a decentralized, zero-install device lifecycle and hardware health protocol built to reclaim ₹1,800+ Crores in missed consumer warranty claims in India.

---

## 🌟 Key Features

1. **⚡ SpecTrace Pulse (Zero-Install WebUSB Diagnostics):**
   - Direct-to-kernel Linux Sysfs queries (`/sys/class/power_supply/battery/cycle_count` and `dumpsys battery`).
   - Reads real battery cycle counts, degradation slopes, and motherboard serials in Chromium with zero apps installed.

2. **💰 Pre-Expiry Warranty Arbitrage:**
   - Detects battery degradation (&lt; 80% capacity) during Month 11 of manufacturer coverage.
   - Auto-generates certified PDF Claim Dossiers for **₹0 free OEM battery replacements** before coverage lapses.

3. **🔊 SpectraTriage (WebAudio Acoustic Diagnostics):**
   - 1 kHz – 10 kHz swept-sine acoustic chirps analyzed via real-time Fast Fourier Transform (FFT).
   - Detects speaker diaphragm tears, dust clogging, and moisture ingress damping before technician dispatch.

4. **📑 GSTIN Modulo-36 Ingestion & Nullifier Vault:**
   - Mathematically verifies 15-digit Indian GSTIN tax invoices in &lt; 1ms to reject forged bills.
   - Computes unique `SHA-256(GSTIN + Serial + Invoice)` duplicate claim nullifiers.

5. **🗺️ SpecTrace Mesh (Decentralized Beckn 2.0 / ONDC Logistics):**
   - Open commerce protocol (`nic2004:52110`) dispatching certified neighborhood micro-technicians in ~15 mins.
   - Eliminates the 30% aggregator middleman tax of centralized platforms.
   - Secured by dual-key UPI Escrow.

---

## 🚀 Quick Start (Local Run)

```bash
# Clone the repository
git clone https://github.com/ksjamwal4268/spectrace.git
cd spectrace

# Start any local HTTP server
python -m http.server 3000

# Open in Chrome / Chromium
open http://localhost:3000
```

---

## 🛠️ Tech Stack
- **Frontend:** HTML5, Aceternity UI Design System, Tailwind CSS, Space Mono & Plus Jakarta Sans.
- **Hardware Telemetry:** WebUSB API, Android Debug Bridge protocol (`@yume-chan/adb`).
- **Audio Diagnostics:** WebAudio API (`AudioContext`, `OscillatorNode`, `AnalyserNode`).
- **Mapping:** Leaflet.js with reverse-engineered Google Maps Vector & Satellite layers (Zero API key dependencies).
- **Commerce Protocol:** Beckn Protocol 2.0 (ONDC Logistics specification).

---

## 📜 License
MIT License • Built for Hackathon Grand-Prix
