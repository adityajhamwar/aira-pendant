# AIRA – The Open-Source AI Pendant That Never Forgets, Never Exploits

**AIRA** is a privacy-first, wearable AI assistant that listens (only when you want), identifies who said what, summarises your conversations, and sets reminders for you. It's fully open-source, works with any AI you choose (local or cloud), and starts at a price anyone can afford.

Inspired by Airavata, the celestial white elephant of Hindu mythology, AIRA embodies wisdom, memory, and absolute trust.

---

## ✨ Features

- 🔒 **Privacy-by-design** – All core processing runs locally. No company servers, no data harvesting.
- 🧠 **Hybrid brain** – Use a small offline AI, or connect your own DeepSeek / ChatGPT / Claude key.
- 👥 **Multi-speaker awareness** – Knows who said what ("Speaker 1", "Speaker 2"…).
- 📝 **Automatic notes & reminders** – Extracts action items and pushes them to your calendar.
- 🌍 **30+ languages** – Auto-detects and works in your language.
- 📈 **Self-learning** – Rate summaries; AIRA gets better for you over time.
- 🐘 **Open-source & affordable** – Hardware and software are free to inspect, modify, and build.

[📖 Full Feature List](docs/FEATURES.md)

---

## 🛠️ Hardware

| Component | Model | Est. Cost |
| :--- | :--- | :--- |
| Microcontroller | Seeed Studio XIAO ESP32S3 Sense | ~€15.39 |
| Microphone | INMP441 MEMS I²S | ~€5.63 |
| RGB LED | WS2812B NeoPixel | ~€0.50 |
| Battery | 3.7V 500mAh Li-Po | ~€4.75 |
| Charger | TP4056 USB-C module | ~€2.39 |
| Button | 6×6mm tactile | ~€0.10 |

[📦 Complete Hardware BOM](docs/HARDWARE.md)

---

## 💻 Software (Fully Open-Source)

| Layer | Tool |
| :--- | :--- |
| Pendant firmware | Owl / Omi |
| Speech-to-text | whisper.cpp |
| Voice activity detection | Silero VAD |
| Speaker diarization | pyannote.audio |
| LLM serving | Ollama |
| Memory | Letta (MemGPT) |
| Orchestration | Pipecat |
| UI | Open WebUI |
| Fine-tuning | Unsloth |

[🧰 Full Software Stack](docs/SOFTWARE.md)

---

## 🚀 Quick Start

> **Detailed build guide coming soon.**

1. **Clone this repo**
   ```bash
   git clone https://github.com/adityajhamwar/aira-pendant.git
   cd aira-pendant
