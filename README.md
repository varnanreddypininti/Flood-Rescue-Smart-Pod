# 🌊 Flood Rescue Smart Pod 🚨

A self-contained, sensor-driven emergency shelter designed to **save lives** during sudden flood disasters. The pod automatically detects danger and acts as a safe, insulated refuge until rescue teams arrive.

---

## 🔍 Overview

Floods strike unexpectedly. Traditional warning systems help—but rarely offer **physical protection**. The **Flood Rescue Smart Pod** bridges that gap.

### ✅ Key Capabilities

- Detects **flood onset** using water level, pressure, and rain sensors
- Automatically inflates airbag to **float above water**
- Seals its door to protect occupants
- Sends **alert signals** (LED + buzzer)
- Operates on **battery backup** during power outages

---

## 🧠 System Architecture

- **Sensors**: DHT11 (Temperature & Humidity), BMP180 (Pressure), Water Level, MPU6050 (Gyro)
- **Controller**: Arduino Uno
- **Actuators**: Diaphragm Pumps, LED Lights, Buzzer
- **Power Source**: 12V Lead Acid Battery
- **Software**: Arduino IDE + Fritzing + Fusion 360

![Block Diagram](documentation/block_diagram.png)

---

## 🛠️ Hardware Used

| Component              | Description                             |
|------------------------|-----------------------------------------|
| Arduino Uno            | Main microcontroller                    |
| DHT11 Sensor           | Temperature & Humidity sensor           |
| BMP180 Sensor          | Air pressure sensor                     |
| MPU6050                | Gyroscope & Accelerometer               |
| Water Level Sensor     | Detects rising water                    |
| R385 Diaphragm Pump    | Inflates airbag for buoyancy            |
| Relay Module           | Switches pumps                          |
| LED & Buzzer           | Visual + Audio alerts                   |
| PCA9548A Multiplexer   | Handles I2C sensor conflicts            |
| Lead Acid Battery      | Backup power during outages             |

---

## 🧪 Working Principle

1. Sensors monitor the environment continuously.
2. Once flood conditions are detected:
   - Buzzer and LED alert is triggered.
   - Pump inflates an **airbag**, lifting the pod.
   - Door seals automatically to prevent water ingress.
3. Gyroscope tracks stability.
4. Status is logged, and alerts are raised.

![Circuit Diagram](documentation/circuit_diagram.png)

---

## 📷 Gallery

Add your setup photos and working videos here for better visualization.

---

## 🚀 Getting Started

### 🔧 Upload Code

1. Open `code/flood_smart_pod.ino` in **Arduino IDE**
2. Select correct board (`Arduino Uno`)
3. Connect via USB and upload

### 📦 Dependencies

Install the following Arduino libraries via Library Manager:

- `Adafruit_MPU6050`
- `Adafruit_BMP085`
- `DHT`

---

## 📌 Future Enhancements

- Add **IoT support** for remote monitoring
- Implement **AI-based flood prediction**
- Enable **GPS + GSM** for live rescue tracking
- Build **multi-occupant pods**

---

## 📄 Documentation

- [📘 Full Report (PDF)](documentation/induction-25_report.pdf)

---

## 💡 Inspired By

- STATIM Pods (USA)
- SIH Hackathons
- Real-life flood disasters in urban areas

---

## 🛟 Stay Safe. Stay Smart.
