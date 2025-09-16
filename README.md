# Gesture-Controlled IoT Rover for Hazardous Environments

## 📌 Overview
This project integrates **Silicon Labs SIWG917** and **ESP8266** to build an IoT system that streams sensor data and controls a rover.

- **SIWG917** acts as a **Wi-Fi HTTP server**, hosting real-time data from the **ICM40627 sensor** (accelerometer, gyroscope).  
- **ESP8266** functions as a **Wi-Fi client**, fetching the data from SIWG917 and printing it to the console.  
- The ESP8266 also controls a **rover** using motor driver logic, where movement is based on sensor values.

## ⚙️ Features
- Real-time **acceleration, and gyro data** via HTTP server.  
- ESP8266 parses server response and **prints values to Serial Monitor**.  
- **Rover control** (forward, backward, left, right) based on accelerometer values.  
- Wi-Fi based communication between SIWG917 and ESP8266.  

## 🛠️ Hardware Used
- Silicon Labs **SIWG917**  
- **ICM40627 IMU Sensor**  
- **ESP8266** 
- L298N Motor Driver + Rover setup  

## 🚀 How It Works
1. SIWG917 initializes Wi-Fi and hosts sensor data at:  
2. ESP8266 connects to the same Wi-Fi, fetches data, and parses JSON response.  
3. Rover movement is decided based on accelerometer X/Y values.
4. The values are shared to a webpage using cloud.
   

