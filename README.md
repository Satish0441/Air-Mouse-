# 🖱️ Air Mouse 

This project transforms an **ESP32** and an **MPU6050 (Gyroscope + Accelerometer)** into a **wireless Air Mouse** using **Bluetooth Low Energy (BLE)**.  
By moving the ESP32 device in the air, the cursor on your computer moves accordingly. Additional buttons are provided for **left click, right click, and scroll** functionality.  

---

## 📷 Circuit Diagram

<img width="3000" height="3480" alt="circuit_image" src="https://github.com/user-attachments/assets/665081fb-c8f2-4d3e-bb3d-ab3406a5c93f" />


---

## ⚡ Features

- Use your **ESP32 as a BLE Mouse**.
- Motion-controlled cursor using **MPU6050 gyroscope**.
- Four physical buttons:
  - **Left Click**
  - **Right Click**
  - **Scroll Up**
  - **Scroll Down**
- Built-in **gyro calibration** for stable control.
- **Moving average filter** to reduce jitter.
- Adjustable **sensitivity and deadzone**.

---

## 🛠️ Components Required

- **ESP32 Dev Module (ESP-WROOM-32)**
- **MPU6050 (Gyroscope + Accelerometer)**
- **4 Push Buttons**
- Jumper wires
- Breadboard or PCB

---

## 🔌 Pin Connections

| ESP32 Pin | MPU6050 Pin | Function         |
|-----------|-------------|------------------|
| 3V3       | VCC         | Power            |
| GND       | GND         | Ground           |
| 22        | SCL         | I²C Clock        |
| 21        | SDA         | I²C Data         |

| ESP32 Pin | Button      | Function         |
|-----------|-------------|------------------|
| 12        | Button 1    | Left Click       |
| 13        | Button 2    | Right Click      |
| 14        | Button 3    | Scroll Up        |
| 27        | Button 4    | Scroll Down      |

---
## Note
 Adjust Sensitivity,ThresholdX and ThresholdY for better control.
## 📦 Arduino Libraries Required

Install the following libraries in Arduino IDE:

**BleMouse**  
   ```arduino
   Sketch → Include Library → Manage Libraries → Search "BleMouse"

