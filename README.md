# HARmony ✨

HARmony is a high-performance, real-time Human Activity Recognition (HAR) application for iOS. It uses built-in smartphone sensors (accelerometer & gyroscope) to classify human activities like walking, climbing stairs, and moonwalking.

<video src="docs/assets/HARmony.mp4" controls width="600"></video>

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

