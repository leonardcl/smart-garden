
# Smart Garden IoT System

![Platform](https://img.shields.io/badge/platform-IoT%20%7C%20Android%20%7C%20Web-blue)
![Language](https://img.shields.io/badge/language-Python%20%7C%20Java%20%7C%20MicroPython-green)
![License](https://img.shields.io/badge/license-MIT-brightgreen)
![Status](https://img.shields.io/badge/status-active-success)

The **Smart Garden IoT System** is designed to help users monitor and control garden conditions remotely. It measures soil moisture, temperature, and light intensity, automating lighting and irrigation based on these readings. The system includes both a web dashboard and an Android application for user control and visualization.

---

## 🌟 Features

- **Real-time Monitoring**: Measures soil moisture, temperature, and light intensity in real time.
- **Automated Control**: Controls garden lighting and irrigation based on sensor readings.
- **Remote Access**: Accessible via both a web dashboard and an Android app for monitoring and control.

---

## 🛠️ Technologies Used

### Hardware
- **Microcontroller**: WeMos
- **Sensors**: DHT11 (Temperature and Humidity)
- **Simulated Light Sensor**: Potentiometer

### Software
- **MQTT**: Message Queuing Telemetry Transport for communication
- **Python**: Backend and web dashboard
- **Java**: Android application
- **Dash & Plotly**: Data visualization for the web

---

## 📈 System Overview

The Smart Garden system reads data from multiple sensors, including soil moisture, temperature, and light intensity. It uses this information to automatically control a pump for irrigation and LED lights for illumination. The system communicates via MQTT, enabling remote monitoring and control through a web-based dashboard and an Android application.

---

## 🚀 Installation

### Prerequisites

1. Install Python 3.x and necessary libraries:
   ```bash
   pip install paho-mqtt dash plotly
   ```
2. Set up Android Studio with necessary SDK and libraries for Android development.
3. Connect the hardware components as described in the circuit diagram in the `/hardware` folder.

### Running the Web Dashboard

1. Navigate to the `src/web_dashboard` directory.
2. Run the dashboard:
   ```bash
   python app.py
   ```
3. Access the dashboard in your browser at `http://localhost:8080`.

### Running the Android App

1. Import the `src/android_app` directory into Android Studio.
2. Configure the MQTT broker settings in `MqttHelper.java`.
3. Build and install the app on your Android device.

---

## 🎮 Usage

- **Web Dashboard**: Monitor real-time sensor data (temperature, humidity, light intensity) and control irrigation and lighting manually.
- **Android App**: Access the same functionalities as the web dashboard directly from your smartphone.

---

## 📂 Repository Structure

```plaintext
smart-garden-iot
├── README.md
├── LICENSE
├── /docs
│   ├── images
│   └── documentation.md
├── /src
│   ├── android_app
│   ├── web_dashboard
│   └── microcontroller_code
├── /hardware
│   ├── circuit_diagram.png
│   └── hardware_specs.md
└── /config
    └── mqtt_config.py
```

---

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please read the `CONTRIBUTING.md` for guidelines.

---

## 💬 Acknowledgements

Special thanks to all open-source projects and libraries that made this project possible.

