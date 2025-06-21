# 🚗🤖 Smart RC Car with Dual Control Modes | سيارت ذكية بنظام تحكم مزدوج

**A multi-modal robotic platform** combining gesture control, autonomous navigation, and pick-and-place functionality.

<div align="center">
  <img src="https://via.placeholder.com/600x400?text=RC+Car+Demo" alt="Project Demo" width="70%">
</div>

## ✨ Key Features

### 🖐️ Gesture Control System
- Arduino-powered hand gesture recognition (CNN model)
- Wireless nRF24L01 communication
- 5 predefined motion commands (forward/backward/left/right/stop)

### 🤖 Autonomous Navigation
- PID-controlled line following (IR sensor array)
- Error < ±2mm from centerline
- Adaptive speed control on curves

### 🏗️ Pick-and-Place Mechanism
- 3DOF servo-powered gripper
- Payload capacity: 200g
- Precision object positioning (±5mm)

### 📱 Bluetooth Remote
- Android control interface
- Manual override capability
- Real-time telemetry display

## 🛠️ Technical Stack
| Component               | Technology Used          |
|-------------------------|-------------------------|
| Microcontroller         | Arduino Mega 2560       |
| Sensors                 | TCRT5000 IR, MPU6050 IMU|
| Actuators               | SG90 Servos, DC Gear Motors |
| Algorithms              | PID Control, CNN Inference |
| Communication           | HC-05 Bluetooth, nRF24L01 |

## 📸 Gallery
<div align="center">
  <img src="https://via.placeholder.com/300?text=Gesture+Control" width="30%">
  <img src="https://via.placeholder.com/300?text=Line+Following" width="30%"> 
  <img src="https://via.placeholder.com/300?text=Gripper+Mechanism" width="30%">
</div>

## 🚀 Getting Started
```bash
# Clone repository
git clone https://github.com/yourusername/rc-car-project.git

# Upload to Arduino
arduino-cli compile --fqbn arduino:avr:mega2560 src/main.ino
