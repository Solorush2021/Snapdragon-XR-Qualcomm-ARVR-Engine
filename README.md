# ⚡ Snapdragon XR Qualcomm AR/VR Engine
### *Hardware-Accelerated Mobile XR Engine with Dynamic Road Generation & Real-Time Performance Profiling*

![Unity](https://img.shields.io/badge/Unity-2022.3%20%2F%20Unity%206-black?style=for-the-badge&logo=unity)
![Architecture](https://img.shields.io/badge/Architecture-DOTS%20%2F%20URP-blue?style=for-the-badge)
![API](https://img.shields.io/badge/API-Vulkan%20%2F%20OpenGL%20ES%203.2-orange?style=for-the-badge)
![Hardware](https://img.shields.io/badge/Hardware-Qualcomm%20Snapdragon%20XR%20%2F%20Adreno-red?style=for-the-badge&logo=qualcomm)
![Performance](https://img.shields.io/badge/Performance-60%2B%20FPS%20%7C%2041%C2%B0C%20Thermal-success?style=for-the-badge)
[![Download APK](https://img.shields.io/badge/Download-Android%20APK%20(133MB)-brightgreen?style=for-the-badge&logo=android)](https://github.com/Solorush2021/Snapdragon-XR-Qualcomm-ARVR-Engine/releases/download/v1.0.0/base.apk)

---

## 📱 Direct APK Download & Quick Start

> **Download Ready**: The pre-built, hardware-accelerated **`base.apk` (133 MB)** is hosted live under [GitHub Releases](https://github.com/Solorush2021/Snapdragon-XR-Qualcomm-ARVR-Engine/releases/tag/v1.0.0).

* **Direct APK Link**: 📥 **[Download base.apk (v1.0.0)](https://github.com/Solorush2021/Snapdragon-XR-Qualcomm-ARVR-Engine/releases/download/v1.0.0/base.apk)**
* **Install via ADB**:
  ```bash
  adb install -r base.apk
  ```

## 🎯 Overview

**Snapdragon XR Qualcomm AR/VR Engine** is a high-performance mobile XR / 3D driving engine developed specifically for **Qualcomm Snapdragon XR** platforms and Adreno mobile GPUs. 

The engine showcases **procedural dynamic road generation**, **off-road terrain physics**, **interactive garage customization**, and a **built-in hardware performance profiler**. By optimizing memory layout and GPU command buffers, the engine sustains **stable 60–90 FPS performance** with a cool **41.0°C thermal envelope** and a low **836MB memory footprint**.

---

## 📸 Visual Showcase & Gameplay Media

### 🏎️ Vehicle Showroom & Procedural Urban Environment

| 🚘 Interactive Garage & Vehicle Showroom | 🏙️ Dynamic Urban City & Road Generation |
| :---: | :---: |
| ![Garage Showroom](media/photo_2026-07-24_13-24-59.jpg) | ![Dynamic City Road Generation](media/photo_2026-07-24_13-26-05.jpg) |
| *3D turntable platform with customizable sports vehicle assets and interactive staging* | *Real-time dynamic road generation with urban building LODs, street lighting, and environment streaming* |

---

### 🏔️ Off-Road Terrain & Real-Time Hardware Performance Profiler

| 📊 Mobile Hardware Performance & Off-Road Terrain Gameplay |
| :---: |
| ![Off-Road Terrain & Hardware Profiler Overlay](media/photo_2026-07-24_13-25-42.jpg) |
| *High-efficiency terrain rendering coupled with live Snapdragon Profiler overlay tracking **60Hz target**, **41.0°C thermal state**, **836MB RAM footprint**, and frame time variance* |

---

## 🏗️ System Architecture & Dynamic Road Engine

```mermaid
flowchart TD
    subgraph Engine Core & Input Layer
        A[Mobile Touch / XR Controller] --> B[Vehicle Physics Controller]
        B --> C[Procedural World & Road Streaming Engine]
    end

    subgraph Dynamic Road & Terrain Generation
        C --> D[Chunk Spawner & Mesh Segment Pooler]
        D --> E[Dynamic LOD & Frustum Occlusion Culling]
    end

    subgraph GPU Acceleration & Qualcomm Hardware Profiler
        E --> F[Vulkan / OpenGLES 3.2 Command Buffers]
        F --> G[Snapdragon Adreno GPU Tile Memory]
        G --> H[Live Hardware Overlay Monitor (60Hz / 41°C / 836MB)]
    end
```

---

## ⚡ Hardware Performance Metrics

Testing executed on **Qualcomm Snapdragon Mobile / XR Reference Hardware** (1080x2196 target render resolution):

| Performance Metric | Measured Value | Engine Target / Benchmark Status |
| :--- | :--- | :--- |
| **Render Resolution** | `1080 x 2196` | Native mobile viewport scaling |
| **Target Refresh Rate** | `60.0 Hz` | Stable locked frame budget |
| **Operating Temperature** | `41.0 °C` | Thermal throttle prevention envelope |
| **System RAM / VRAM Usage** | `836 MB` | Low-footprint zero-GC memory allocation |
| **Road Generation Latency** | `< 1.2 ms` | Procedural segment chunk streaming |
| **Graphics API** | `Vulkan / OpenGL ES 3.2` | Hardware-accelerated multi-threaded draw calls |

---

## 🚀 GitHub Releases: APK & Video Demonstration Setup

> [!IMPORTANT]
> **GitHub Storage & LFS Recommendations for Large Binaries**:
> Standard Git repositories restrict individual files over **100MB**. To keep the repository lightweight and maintain clean Git commit history, compiled Android binaries (`base.apk`) and high-bitrate video clips are stored in **GitHub Releases**.

### 📱 Installing `base.apk`

1. Navigate to the project **[GitHub Releases Page](../../releases)**.
2. Download `base.apk` (or `Snapdragon_XR_Engine_v1.0.apk`).
3. Connect your Android / Snapdragon XR headset via USB and install using ADB:
   ```bash
   adb install -r base.apk
   ```

### 🎥 High-Frame-Rate Video Demonstration Placement
- **Release Assets**: Upload full 60FPS high-resolution MP4 video walkthroughs to the corresponding GitHub Release release notes.
- **Embedded Preview**: You can link YouTube / GitHub release video embeds directly inside this README section:
  ```markdown
  [![Watch Snapdragon XR Demo](https://img.youtube.com/vi/YOUR_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)
  ```

---

## 🛠️ Build & Installation Guide

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Solorush2021/Snapdragon-XR-Qualcomm-ARVR-Engine.git
   ```
2. **Open in Unity**:
   - Required Version: **Unity 2022.3 LTS** or **Unity 6**.
   - Platform Target: **Android (ARM64)**.
3. **Configure Project Settings**:
   - Set Graphics API to **Vulkan** (Primary) with fallback to **OpenGL ES 3.2**.
   - Enable **Multithreaded Rendering** and **Universal Render Pipeline (URP)**.

---

## 👨‍💻 Author

**Vipul Kumar**  
*AI & Heterogeneous Edge Systems Engineer*  
* [LinkedIn](https://linkedin.com/in/vipul-kumar-4388801a7)  
* [GitHub](https://github.com/Solorush2021)  
* Email: vipulpower@gmail.com
