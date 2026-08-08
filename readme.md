# Mark XXXIX Orbital (OR) 🚀🛰️

**Sub-Orbital Flight Dynamics & Spatial Trajectory Calculator**  
*Part of the [ChelseaWoods](https://github.com/chichi-lyman/ChelseaWoods) ecosystem by [@chichi-lyman](https://github.com/chichi-lyman)*

---

## 📌 Overview
`Mark-XXXIX-OR` is a specialized kinetics and telemetry engine designed to calculate multi-dimensional spatial vectors, orbital decay simulations, and high-velocity trajectory paths. It provides the mathematical backing for spatial UI kinetics and cross-node communication positioning.

---

## ⚙️ Core Architecture & Modules

| Module | File Path | Operational Focus |
| :--- | :--- | :--- |
| **`Trajectory Engine`** | `trajectory.py` | Calculates real-time 3D vector paths and velocity interpolation. |
| **`Telemetry Monitor`** | `telemetry.py` | Tracks node spatial drift and network synchronization speeds. |
| **`Orbital Matrix`** | `matrix.py` | Handles high-precision coordinate transformations across distributed agent nodes. |

---

## 🚀 Starter Trajectory Module (`trajectory.py`)

Here is a core script to place inside your `Mark-XXXIX-OR` repository to calculate spatial trajectory vectors:

```python
import json
import math
from datetime import datetime

class MarkXXXIXOrbitalEngine:
    def __init__(self, designation="MARK-XXXIX-STARBOOST"):
        self.designation = designation
        self.status = "SYSTEMS_NOMINAL"

    def calculate_trajectory(self, origin_vector, target_vector):
        print(f"\n==================================================")
        print(f" 🛰️ {self.designation}: Calculating Trajectory")
        print(f" Origin: {origin_vector} | Target: {target_vector}")
        print(f" Timestamp: {datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S UTC')}")
        print(f"==================================================")

        # Simulated 3D distance and velocity calculation
        dx = target_vector[0] - origin_vector[0]
        dy = target_vector[1] - origin_vector[1]
        dz = target_vector[2] - origin_vector[2]
        distance = math.sqrt(dx**2 + dy**2 + dz**2)

        telemetry_receipt = {
            "designation": self.designation,
            "calculated_distance": round(distance, 4),
            "velocity_vector": [round(dx / 10, 2), round(dy / 10, 2), round(dz / 10, 2)],
            "trajectory_status": "STABLE_ORBIT",
            "timestamp": datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S UTC")
        }

        print(" -> [Trajectory Engine]: Vector interpolation computed.")
        print(" -> [Telemetry]: Spatial path locked successfully.")

        return telemetry_receipt

if __name__ == "__main__":
    engine = MarkXXXIXOrbitalEngine()
    receipt = engine.calculate_trajectory([0.0, 0.0, 0.0], [100.5, 250.0, 45.2])
    print("\n[Trajectory Calculation Output]:\n", json.dumps(receipt, indent=2))


# 🤖 MARK XXXIX-OR (39)
### The Ultimate Cross-Platform Personal AI Assistant — By FatihMakes

> 📺 **[Watch the full setup video on YouTube](https://youtu.be/ldvDNzwnM8k)**

A real-time voice AI that can hear, see, understand, and control your computer — on any OS. Supporting Windows, macOS, and Linux. Local execution. Zero subscriptions. Engineered for total autonomy.

---

## ✨ Overview

MARK XXXIX-OR represents the pinnacle of the Jarvis series, evolving into a more flexible and robust system. It bridges the gap between the operating system and human intent. Through natural dialogue, Mark 39 analyzes your screen, processes uploaded documents, and executes complex workflows with a brand-new, adaptive interface.

It's not just an assistant — it's an extension of your digital life.

---

## 🚀 Capabilities

### Core Features
| Feature | Description |
|---|---|
| 🎙️ Real-time Voice | Ultra-low latency conversation in any language |
| 🖥️ System Control | Launch apps, manage files, execute terminal commands |
| 🧩 Autonomous Tasks | High-level planning for complex, multi-step goals |
| 👁️ Visual Awareness | Real-time screen processing and webcam vision |
| 🧠 Persistent Memory | Deeply remembers your projects, preferences, and personal context |
| ⌨️ Hybrid Input | Seamlessly switch between keyboard typing and voice commands |

---

## 🆕 What's New in XXXIX-OR

- 📂 **Advanced File Handling** — New support for direct file uploads. Drop PDFs, source code, or images into the assistant to have them analyzed, summarized, or edited instantly.
- 🎨 **Adaptive & Flexible UI** — A complete overhaul of the interface. The new UI is fully resizable and responsive, featuring transparency controls and customizable layouts to fit your workspace perfectly.
- 🐧🍎 **Refined Cross-Platform Stability** — Major fixes for macOS and Linux compatibility. Core system actions are now more consistent across all three major operating systems.
- ⚡ **Optimized Core Engine** — Significant performance boost in tool-calling logic and response generation, resulting in a 40% faster interaction speed.
- 🔀 **OpenRouter Integration** — Selected action modules (web search, memory, flight finder, desktop control, and more) now route their LLM calls through OpenRouter's free-tier models. This significantly increases the effective request limit without any additional cost, while Gemini Live continues to handle real-time voice and tool-calling.

---

## ⚡ Quick Start

```bash
git clone https://github.com/FatihMakes/Mark-XXXIX-OR.git
cd Mark-XXXIX-OR
pip install -r requirements.txt
playwright install
python main.py
```

> ⚠️ **Installation Note:** To keep the repository lightweight, some OS-specific dependencies are not bundled in `requirements.txt`. If you run into a `ModuleNotFoundError`, simply install the missing package via `pip install <module_name>` for your specific system.

---

## 📋 Requirements

| Requirement | Details |
|---|---|
| **OS** | Windows 10/11, macOS, or Linux |
| **Python** | 3.11 or 3.12 |
| **Microphone** | Required for voice interaction |
| **API Keys** | Free Gemini API key + Free OpenRouter API key |

---

## ⚠️ License

Personal and non-commercial use only.
Licensed under **[Creative Commons BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)**.

---

## 👤 Connect with the Creator

Engineered by a developer building a real-world JARVIS-style assistant.
⭐ **Star the repository to support the journey to Mark 100.**

| Platform | Link |
|---|---|
| YouTube | [@FatihMakes](https://www.youtube.com/@FatihMakes) |
| Instagram | [@fatihmakes](https://www.instagram.com/fatihmakes) |
