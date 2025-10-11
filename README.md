# HW-IntelN100-Mini-AI-PC

<div align="center">

# 💻 HW-IntelN100-Mini-AI-PC

<img src="https://github.com/user-attachments/assets/43808935-255c-4f9e-9415-c40cd7b88f74" width="480px" alt="Mini AI PC"/>

**A custom Intel N100-based Mini AI PC — compact, quiet, and powerful for edge AI and embedded applications.**

---

</div>

## 🧭 Overview

The **Intel N100 Mini AI PC** is a small-form-factor system designed and built by **Ceyhun Pempeci** to combine **industrial reliability**, **AI-ready performance**, and **maker-friendly modularity**.  
It’s ideal for embedded AI, robotics, computer vision, IoT gateways, and automation systems where power efficiency and expandability matter.

This project includes the **complete hardware documentation** and a **PDF assembly guide** for those who wish to replicate or adapt the design.

📄 [**Assembly Guide → N100PC.pdf**](./N100PC.pdf)

---

## ⚙️ Specifications

| Category | Details |
|-----------|----------|
| **Processor** | Intel N100 (4 Cores / 4 Threads, Alder Lake - E, Turbo up to 3.4 GHz) |
| **Graphics** | Intel UHD Graphics (24 EUs) — supports AI acceleration and 4K video |
| **Memory** | DDR4 / LPDDR5 support (depending on configuration) |
| **Storage** | M.2 NVMe SSD / eMMC / SATA options |
| **Connectivity** | USB 3.2 Gen 2 × 4, USB-C, HDMI 2.0, Ethernet (2.5 Gb PoE optional), Audio Jack |
| **Expansion** | M.2 Key-E for Wi-Fi / Bluetooth / AI Accelerators |
| **Power** | 12 V DC Input (min 25 W) |
| **Cooling** | Compact aluminum heatsink + optional quiet fan |
| **Operating Systems** | Ubuntu 22.04, Debian 12, Armbian, and other Linux distributions |
| **Use Cases** | Edge AI camera systems, IoT servers, robotics controllers, and prototyping platforms |

---

## 🧰 Setup & Usage

### 🪛 Assembly
Follow the [**N100PC.pdf**](./N100PC.pdf) manual for:
- Mounting the motherboard, SSD, and cooling system  
- Installing RAM and M.2 modules  
- Connecting power, I/O, and front panel cables  

### 💽 Operating System Installation
1. Create a bootable USB with **Ubuntu 22.04** or **Debian 12**.  
2. Plug it into the PC and power on.  
3. Install OS on your NVMe SSD or eMMC.  

### ⚙️ Post-Installation
```bash
sudo apt update && sudo apt upgrade
sudo apt install python3-pip git
pip3 install torch torchvision onnxruntime opencv-python
