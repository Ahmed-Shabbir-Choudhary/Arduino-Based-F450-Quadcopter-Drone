# 🚁 Arduino-Based F450 Quadcopter — Wing Sky Rider

> A fully functional quadcopter built on an F450 frame, controlled via Arduino Uno with real-time IMU-based flight stabilization.

![Platform](https://img.shields.io/badge/Platform-Arduino%20Uno-blue)
![Course](https://img.shields.io/badge/Course-Electric%20Network%20Analysis-green)
![University](https://img.shields.io/badge/University-NUST-red)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Overview

**Wing Sky Rider** is an Arduino-based quadcopter designed and built as a semester project for the Electric Network Analysis (EE-211) course at NUST SEECS. The project involved full system integration — from structural assembly and motor calibration to flight controller programming and sensor fusion — resulting in a stable, flyable quadcopter.

---

## ⚙️ Components Used

| Component | Description |
|---|---|
| Arduino Uno | Main flight controller (ATmega328P) |
| MPU-6050 | 6-axis IMU — 3-axis gyroscope + 3-axis accelerometer |
| F450 Frame | Lightweight quadcopter frame, 450mm diagonal |
| A2212 1400KV Brushless Motors | High-efficiency DC brushless motors (×4) |
| 30A ESC | Electronic Speed Controllers for motor control (×4) |
| 1045 Propellers | 10-inch diameter, 4.5-inch pitch propellers (×4) |
| LiPo Battery | Power source for motors and electronics |

---

## 🧠 System Architecture

```
LiPo Battery
     │
     ▼
Power Distribution Board
     │
  ┌──┴──┐
  ESC × 4
  │
Brushless Motors × 4
     
MPU-6050 (IMU)
     │
     ▼
Arduino Uno (Flight Controller)
     │
  PID Stabilization Logic
     │
  Motor Speed Commands
```

---

## 🔧 Key Features

- **Real-time flight stabilization** using MPU-6050 gyroscope and accelerometer data
- **PID control logic** implemented on Arduino Uno for stable hover and maneuverability
- **F450 symmetric frame** ensuring balanced weight distribution across all four arms
- **Modular design** allowing easy replacement of motors, ESCs, and propellers
- **Compatible with FPV cameras** and additional payload modules

---

## 📐 Methodology

1. Assembled the F450 frame and mounted A2212 brushless motors on each arm
2. Wired 30A ESCs to the power distribution board and connected to Arduino
3. Integrated MPU-6050 IMU via I2C for real-time orientation data
4. Programmed Arduino Uno with flight stabilization logic using sensor fusion
5. Calibrated ESCs and performed motor spin tests
6. Conducted flight tests and tuned PID parameters for stable flight

---

## 📁 Repository Structure

```
Arduino-Based-F450-Quadcopter-Drone/
├── code/
│   └── quadcopter_code.docx       # Flight controller code
├── media/
│   └── demo_video.mp4             # Project demo video
│   └── hardware_photo1.jpg        # Hardware assembly photo
│   └── hardware_photo2.png        # Circuit/wiring photo
└── README.md
```

---

## 👥 Team

| Name | Roll No |
|---|---|
| Ahmed Shabbir Choudhary | 465206 |
| Muhammad Husnain Shabir | 455436 |
| Mansoor Ahmed Rind | 460643 |
| Muhammad Obaid | 460745 |
| Muhammad Ibraheem | 414115 |
| Muhammad Hashir | 469981 |
| Iqra Hayat | 455461 |
| Muhammad Umer Khawaja | 468867 |

---

## 🏫 Course Information

- **Course:** Electric Network Analysis (EE-211)
- **Instructor:** Dr. Ahsan Azhar
- **University:** NUST SEECS, Islamabad
- **Semester:** Spring 2024

---

## 🚀 Future Enhancements

- Integrate GPS module for autonomous waypoint navigation
- Add FPV camera for real-time aerial footage
- Implement wireless telemetry for live flight data monitoring
- Upgrade to a dedicated flight controller (e.g., APM or Pixhawk)
