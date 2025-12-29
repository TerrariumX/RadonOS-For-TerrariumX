# RadonOS

RadonOS is a lightweight, modular operating system built for modern ESP32-based boards.

It is the core OS behind the **TerrariumX ecosystem**, but it can also be used as a standalone platform for advanced ESP32 projects that need reliability, structure, and a clean local interface.

RadonOS is designed with a simple idea in mind: **treat embedded systems like real systems**, not disposable firmware.

---

## ✨ What RadonOS is about

RadonOS focuses on:

* 🧩 **Modularity** – services are independent and restartable
* 🌐 **Local-first operation** – no cloud required
* 🔌 **MQTT-native design** – easy Home Assistant and automation integration
* 🖥️ **Modern WebUI** – animated, responsive, and optimized for embedded hardware
* 🛠️ **Long-term support** – hardware and software designed to evolve together
* 🔁 **Multi-MCU awareness** – ready for boards with main MCU + secondary / BIOS MCU

---

## 🧩 Supported Boards (Launch)

### Waveshare boards

| Board                   | MCU      | Notes                    |
| ----------------------- | -------- | ------------------------ |
| ESP32-P4-Module-DEV-KIT | ESP32-P4 | Full-featured dev kit    |
| ESP32-P4-Nano           | ESP32-P4 | Compact form factor      |
| ESP32-P4-WIFI           | ESP32-P4 | WiFi-enabled variant     |
| ESP32-P4-ETH            | ESP32-P4 | Ethernet-enabled variant |

### TerrariumX boards

| Board     | MCU                        | Notes                          |
| --------- | -------------------------- | ------------------------------ |
| **TXDK0** | ESP32-P4 (dual-MCU design) | Reference board for TerrariumX |

### General DevKits

| Family   | Supported | Notes                   |
| -------- | --------- | ----------------------- |
| ESP32-P4 | ✅         | Primary target platform |
| ESP32-S3 | ✅         | Supported at launch     |
| ESP32-S2 | ✅         | Supported at launch     |
| ESP32-C6 | 🛠️         | Supported after 1.2 and by custom version only|
| ESP32-C5 | 🛠️         | Supported after 1.2 and by custom version only|
| ESP32-C3 | 🛠️         | Supported after 1.2 and by custom version only|
| ESP32-C2 | 🛠️         | Supported after 1.2 and by custom version only|
| ESP32    | 🛠️         | Supported in 1.1 (Attention to high loads)|
| ESP8266  | ❌         | On EOL by Espressif     |

> More boards and families will be added over time as RadonOS expands.

---

## 🧠 Architecture (high level)

RadonOS uses a **service-oriented architecture**:

* Core kernel
* Hardware Abstraction Layer (HAL)
* Independent system services (GPIO, Network, Storage, Sensors, Power, etc.)
* Local WebUI server
* MQTT bridge

Each service can be started, stopped, or restarted independently, improving reliability and making debugging much easier compared to monolithic firmware designs.

---

## 🌐 WebUI

RadonOS includes a fully local WebUI that runs directly on the device:

* Modern Material-inspired design
* Smooth animations and micro-interactions
* System monitoring and diagnostics
* Power and service control
* OTA and update management (experimental)

Despite the visual complexity, the WebUI is designed to stay lightweight and efficient, making it suitable even for constrained embedded hardware.

---

## 🔄 Updates & OTA

RadonOS supports **GitHub-based update workflows** (experimental):

* Version checks via remote JSON files
* Firmware and WebUI updates
* Designed for local network environments

> OTA features are under active development and should be considered experimental.

---

## 🚧 Project Status

RadonOS is under **active development**.

This means:

* Rapid iteration
* New features arriving frequently
* Possible breaking changes in early versions

If you are using RadonOS for testing or development, feedback is highly appreciated.

---

## 🤝 Contributing

Contributions are welcome.

You can help by:

* Testing on supported boards
* Reporting issues
* Improving documentation
* Adding support for new hardware

Feel free to open issues or pull requests.

---

## 🔓 License

RadonOS is fully **open source** and free to use.

See the LICENSE file for detailed license information.
