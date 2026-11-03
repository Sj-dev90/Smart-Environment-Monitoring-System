# 🌐 FocusAir OS
> *A futuristic, cyberpunk-styled smart environmental monitoring system and tactical telemetry dashboard.*

![FocusAir OS Banner](https://img.shields.io/badge/STATUS-OPERATIONAL-00ff66?style=for-the-badge&logo=terminal&logoColor=00ff66)
![Tech Stack](https://img.shields.io/badge/STACK-HTML5%20|%20CSS3%20|%20JS%20|%20Chart.js-b026ff?style=for-the-badge)
![IoT Cloud](https://img.shields.io/badge/BACKEND-Adafruit%20IO-yellow?style=for-the-badge&logo=adafruit&logoColor=black)

---

## ⚡ Overview

**FocusAir OS** is an immersive, web-based IoT dashboard designed to monitor and evaluate real-time environmental telemetry (Particulate Density/AQI, Atmospheric Saturation, and Thermal Metrics). Built with a high-end sci-fi aesthetic, it bridges local sensor hardware with cloud infrastructure to deliver not just raw data, but actionable **tactical recovery and cognitive health advisories**.

---

## 🚀 Key Features

*   **🔐 Operator Authentication:** Secure system initialization sequence allowing operators to log in and lock/unlock the main terminal interface.
*   **📊 Live Telemetry Array:** Real-time data cards updating dynamically via the Adafruit IO REST API.
*   **📈 Dynamic Chart.js Integration:** Smooth, real-time line graphs tracking historical trends for AQI, Humidity, and Temperature without lagging the UI.
*   **💻 Data Matrix Terminal Log:** A scrolling technical ingestion log displaying live data packets complete with exact timestamp tracking.
*   **🛡️ Bio-Recovery Control Module:** Interactive system controls including a faked HEPA Air Scrubber "Purge Cycle" sequence and level-restricted thermal overrides.
*   **🧠 Tactical Recovery & Advisory System:** An intelligent diagnostic engine that evaluates incoming environmental conditions in real time to calculate:
    *   **Cognitive Load:** Assessing focus drift, micro-particulate neurological impact, and heat fatigue.
    *   **Physical Directives:** Providing hydration alerts and physical exertion caps.
    *   **Egress & Safe-Zone Routing:** Automatically recommending tactical escape routes and clean-room sectors based on live hazard thresholds.

---

## 🛠️ System Architecture

1.  **Hardware / Local Script (`bridge.py`):** Sensors capture physical environmental data locally and push telemetry packets to the cloud.
2.  **Cloud Broker (`Adafruit IO`):** Acts as the central data registry holding public feeds for `temperature`, `humidity`, and `aqi`.
3.  **Web Frontend (`GitHub Pages`):** A single-page application (SPA) built using vanilla JavaScript and CSS that safely pulls data via secure API headers and renders the UI.

---

## 📂 Project Structure

```text
/
├── index.html        # Complete Single-Page Application (UI, CSS, and Client Logic)
├── bridge.py         # Local Python script pushing sensor data to Adafruit IO
└── README.md         # Project Documentation
