# IoT Based Health Monitoring System (Heart Rate & SpO2)

## Project Overview
This project is an IoT-based health monitoring system that measures heart rate (BPM) and blood oxygen level (SpO2) using sensors and sends the data to the Blynk app in real time.

It is designed for remote patient monitoring and basic health tracking.

---

## Components Used
- ESP8266 (NodeMCU)
- Pulse Sensor (for Heart Rate)
- MAX30100 / MAX30102 (for SpO2 & Heart Rate)
- WiFi Connection
- Blynk IoT Platform

---

## Working Principle
1. The pulse sensor detects heartbeats and calculates BPM.
2. The MAX30100 sensor measures:
   - Heart Rate
   - Blood Oxygen (SpO2)
3. ESP8266 processes sensor data.
4. Data is sent to the Blynk app via WiFi.
5. User can monitor health parameters in real-time.

---

## Blynk Integration
- Virtual Pin V1 : Heart Rate (BPM)
- Virtual Pin V2 : SpO2 (%)

---

## Circuit Connections
### Pulse Sensor
- VCC : 3.3V
- GND : GND
- Signal : A0

### MAX30100
- SDA : D2
- SCL : D1
- VCC : 3.3V
- GND : GND

---

## Code Features
- Real-time BPM detection
- SpO2 monitoring
- WiFi-based IoT communication
- Serial monitoring for debugging

---

## Important Notes
- Update WiFi credentials in code:
  ```cpp
  char ssid[] = "YourNetworkName";
  char pass[] = "YourPassword";
