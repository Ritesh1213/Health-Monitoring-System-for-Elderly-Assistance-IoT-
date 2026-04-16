# Health-Monitoring-System-for-Elderly-Assistance-IoT-
Smart wearable fall detection band using ESP32-C3 SuperMini and MPU6050 sensor. It monitors motion and detects falls based on sudden impact and orientation change. On detection, it sends real-time alerts via Wi-Fi to caregivers, enabling quick response and improving elderly safety.
📌 Overview

This project is a hybrid health monitoring and fall detection system designed for elderly assistance. It combines a wearable IoT device with CCTV-based computer vision to provide accurate and reliable monitoring.

The wearable band, powered by the ESP32-C3 SuperMini, continuously tracks vital health parameters such as heart rate, SpO2, body temperature, and motion. In parallel, a computer vision system analyzes CCTV footage to detect falls, ensuring higher accuracy and reducing false positives.

🚀 Features
🧠 Dual fall detection (Sensor-based + Computer Vision)
❤️ Heart rate monitoring (MAX sensor)
🫁 SpO2 (blood oxygen level) tracking
🌡️ Body temperature monitoring (LM35)
📡 Real-time data transmission via Wi-Fi
🎥 CCTV-based fall detection using computer vision
🚨 Instant alert system for caregivers
⌚ Wearable handband design
🧰 Hardware Components
ESP32-C3 SuperMini
MPU6050 (Accelerometer + Gyroscope)
MAX30102 / MAX30100 (Heart Rate & SpO2 Sensor)
LM35 Temperature Sensor
Li-ion / Li-Po Battery
TP4056 Charging Module
💻 Software & Technologies
Arduino IDE / PlatformIO
Embedded C (ESP32)
Python (for computer vision)
OpenCV (fall detection via CCTV)
Wi-Fi / IoT Communication
Cloud Platform (optional: Blynk / Firebase / ThingSpeak)
🧠 System Architecture
Wearable device collects:
Motion data (MPU6050)
Heart rate & SpO2 (MAX sensor)
Body temperature (LM35)
ESP32 processes sensor data and detects abnormalities
CCTV camera feed is analyzed using OpenCV for fall detection
Sensor-based + vision-based results are combined
Alerts are sent via Wi-Fi to caregivers or cloud dashboard
⚙️ Fall Detection Methods
📍 Sensor-Based Detection
Detect sudden acceleration (impact)
Analyze orientation change using gyroscope
Trigger fall event if thresholds are exceeded
🎥 Computer Vision Detection
Human detection from CCTV feed
Posture analysis (standing → lying transition)
Fall confirmation using frame analysis
📂 Project Structure
Health-Monitoring-System/
│── hardware/
│   ├── circuit_diagram.png
│   └── wearable_design.jpg
│
│── firmware/
│   └── esp32_code.ino
│
│── computer_vision/
│   └── fall_detection.py
│
│── docs/
│   └── system_architecture.md
│
│── README.md
⚙️ Setup & Installation
🔧 Hardware Setup
Connect MPU6050 via I2C
Connect MAX30102 sensor
Connect LM35 to analog pin
Power using battery module
💻 Firmware Setup
Install Arduino IDE
Add ESP32 board support
Install required libraries
Upload code to ESP32-C3
🎥 Computer Vision Setup
Install Python
Install OpenCV:
pip install opencv-python
Run fall detection script:
python fall_detection.py
📸 Demo & Results
<img width="496" height="307" alt="image" src="https://github.com/user-attachments/assets/a5c54614-d779-44be-a980-a355ae5fe568" />

<img width="344" height="220" alt="image" src="https://github.com/user-attachments/assets/43dca3d1-3395-402c-be8a-148e3cf2f4eb" />

🎯 Future Improvements
📱 Mobile app integration
🧠 AI/ML-based fall detection
📍 GPS tracking
🔔 Buzzer/vibration alerts
🔋 Power optimization
📊 Applications
Elderly care systems
Smart healthcare IoT
Remote patient monitoring
Assisted living environments
🤝 Contribution

Feel free to fork this repository and contribute!

📜 License

MIT License

🙌 Acknowledgements
Arduino & ESP32 community
OpenCV library
Open-source IoT platform
