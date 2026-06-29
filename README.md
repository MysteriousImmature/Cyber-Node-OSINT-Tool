# 🛡️ Cyber Node Pro | OSINT Terminal

**Cyber Node Pro** is a high-performance, browser-based Open Source Intelligence (OSINT) aggregator. It provides security analysts with a centralized "glass-pane" view for investigating malicious IPs, Hashes, and Domains across multiple threat intelligence platforms simultaneously.

---

## 🌐 Live Access

The terminal is deployed and accessible at the following nodes:

* **[Main Production Node](https://mysteriousimmature.github.io/Cyber-Node-OSINT-Tool/)**

---

## 🚀 Features

* **Multi-Engine Correlation:** Query VirusTotal, AlienVault OTX, Hybrid Analysis, and ThreatFox from a single input.
* **Real-time Intelligence:** Live API integration for up-to-the-minute threat verdicts.
* **Adaptive UI:** Cyberpunk-inspired SOC interface using Tailwind CSS and Lucide icons with glassmorphism effects.
* **Persistent Sessions:** Built-in `localStorage` support to save your last scan results and maintain session states.
* **Integrated Proxy Bridge:** Toggleable CORS-Anywhere integration to bypass browser-side API restrictions.
* **System Lock:** Basic front-end access control to prevent unauthorized terminal use.

---

## 🛠️ Setup & Configuration

Since this is a standalone client-side application, setup is minimal.

### 1. Get Your API Keys
You will need to register for free (or premium) API keys from the following providers:
* [VirusTotal API](https://www.virustotal.com/)
* [AlienVault OTX](https://otx.alienvault.com/)
* [Hybrid Analysis](https://www.hybrid-analysis.com/)

### 2. Configure the Script
Locate the `API_CONFIG` constant in the `<script>` section of the HTML file and insert your keys:

```javascript
const API_CONFIG = {
      VIRUSTOTAL_API_KEY: 'YOUR_KEY_HERE',
      HYBRID_ANALYSIS_API_KEY: 'YOUR_KEY_HERE',
      ALIENVAULT_OTX_API_KEY: 'YOUR_KEY_HERE',
      USE_PROXY: true 
};
