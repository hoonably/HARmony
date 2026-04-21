# HARmony ✨
<a href="https://github.com/hoonably/HARmony"><img src="https://img.shields.io/static/v1?label=Project&message=GitHub&color=blue"></a>
<a href="https://hoonably.github.io/HARmony"><img src="https://img.shields.io/static/v1?label=Project&message=PDF&color=red"></a>
<a href="https://hoonably.github.io/HARmony/assets/HARmony.mp4"><img src="https://img.shields.io/badge/Project-Video-2ea44f?logo=video&logoColor=white"></a>

> 🥇 Best Award - Ranked 1st in the course.

HARmony is a high-performance, real-time Human Activity Recognition (HAR) application for iOS. It uses built-in smartphone sensors (accelerometer & gyroscope) to classify human activities like walking, climbing stairs, and moonwalking.

<p align="center">
  <img src="analysis/report_figures/raw_signals_group1.png" alt="Raw signal preview group 1" width="49%">
  <img src="analysis/report_figures/raw_signals_group2.png" alt="Raw signal preview group 2" width="49%">
</p>

Sensor previews from the analysis pipeline show synchronized accelerometer and gyroscope patterns across representative activity groups.

<video src="https://github.com/user-attachments/assets/ca8921c8-d845-445a-a1a8-feb108677013" width="100%" controls></video>

## 🚀 Key Features

- **Real-time Activity Detection**: High-density inference using optimized rule-based classification.
- **Sensor Data Collection**: Record synchronized inertial data (acc + gyro) for further tuning.
- **Live Visualization**: Smooth chart representation of raw sensor signals.
- **Optimized for iOS**: Pure Swift implementation with focus on battery efficiency and responsiveness.

## 🛠️ How to Reproduce

Follow these simple steps to clone and run the project:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/hoonably/HARmony.git
   cd HARmony
   ```

2. **Open in Xcode**
   - Double-click `HARmony.xcodeproj` to open the project.
   - Recommended version: **Xcode 15+**.

3. **Configure Signing (Personalized)**
   - Open `Config.xcconfig` and update `DEVELOPMENT_TEAM` and `PRODUCT_BUNDLE_IDENTIFIER` with your own details.
   - *Note: Update Config.xcconfig with your own credentials to build & run.*

4. **Build and Run**
   - Select a physical iPhone (recommended for sensor access) or a Simulator.
   - Press **Cmd + R** to build and run.

## 📂 Project Structure

- `ActivityClassifier.swift`: The core logic for rule-based motion classification.
- `MotionManager.swift`: Handles communication with CoreMotion and provides synchronized sampling.
- `CollectView.swift`: UI for recording sensor data with automated countdowns.
- `DetectView.swift`: Real-time activity recognition interface.
- `docs/`: Project documentation and media assets (demo video, PDF guide).

