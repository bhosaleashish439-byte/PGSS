# Personal Guardian Safety System (PGSS)

A wearable fall detection device built on ESP32, utilizing an on-device Convolutional Neural Network (CNN) for real-time fall detection. The system features Telegram emergency alerts with GPS location tracking and a dedicated web dashboard to log fall history.

## 🚀 Key Features
* **Real-Time Edge AI:** Executes a trained CNN model directly on the ESP32 for immediate fall detection without relying on continuous cloud processing.
* **Telegram Emergency Alerts:** Automatically dispatches instant notifications containing real-time GPS coordinates to designated contacts when a fall is detected.
* **Gmail Emergency alerts:**Automatically dispatches instant notifications containing real-time GPS coordinates to designated contacts when a fall is detected.
* **Web Dashboard Integration:** Logs and displays fall history on a centralized web interface for continuous monitoring and review.
* **Custom Memory Allocation:** Utilizes a custom partition scheme to efficiently accommodate the embedded machine learning model.

## 🛠️ Technologies & Hardware
* **Microcontroller:** ESP32
* **Development Environment:** PlatformIO
* **Languages:** C, C++
* **Notifications:** Telegram Bot API and gmail
* **Machine Learning:** Embedded CNN

## 📂 Repository Structure
* `main.cpp` — Core application logic, sensor data acquisition, and inference execution.
* `pgss_model.h` — The exported, on-device CNN model header file.
* `partitions.csv` — Custom memory partition table defining space for the ESP32 application and ML model.
* `platformio.ini` — PlatformIO project configuration, build environments, and library dependencies.
* `LICENSE` — MIT License documentation.
