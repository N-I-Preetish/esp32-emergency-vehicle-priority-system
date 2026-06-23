# ESP32 Emergency Vehicle Priority System

## Overview

This project demonstrates a smart traffic signal system using two ESP32 boards and ESP-NOW wireless communication. An emergency vehicle unit equipped with a sound sensor detects high-intensity siren sounds and wirelessly sends an emergency signal to the traffic signal unit. Upon receiving the signal, the traffic light automatically switches to green, allowing emergency vehicles to pass safely and without delay.

## Features

* Wireless communication using ESP-NOW
* Emergency vehicle sound detection
* Automatic traffic signal control
* Emergency vehicle priority system
* Real-time traffic signal switching
* Low-cost prototype for smart city applications
* Easy to build and expand

## Components Required

### Emergency Vehicle Unit

* ESP32 Development Board
* Sound Sensor Module (KY-037 / KY-038)
* Breadboard
* Jumper Wires
* USB Cable

### Traffic Signal Unit

* ESP32 Development Board
* Red LED
* Yellow LED
* Green LED
* 3 × 220Ω Resistors
* Breadboard
* Jumper Wires
* USB Cable

## Pin Connections

### Emergency Vehicle Unit

| Sound Sensor | ESP32   |
| ------------ | ------- |
| VCC          | 3.3V    |
| GND          | GND     |
| AO           | GPIO 34 |

### Traffic Signal Unit

| Component  | ESP32 Pin |
| ---------- | --------- |
| Red LED    | GPIO 25   |
| Yellow LED | GPIO 26   |
| Green LED  | GPIO 27   |

## Working Principle

1. The sound sensor continuously monitors surrounding sound levels.
2. When the detected sound level exceeds the predefined threshold, the emergency vehicle ESP32 detects the siren sound.
3. The emergency vehicle ESP32 sends an emergency message using ESP-NOW.
4. The traffic signal ESP32 receives the emergency signal.
5. The traffic signal immediately switches to green.
6. The green signal remains active for 10 seconds.
7. The yellow signal turns on for 2 seconds.
8. The system automatically returns to the red signal state.

## Software Used

* Arduino IDE
* ESP32 Board Package
* ESP-NOW Library
* WiFi Library

## Project Structure

```text
ESP32-Emergency-Vehicle-Priority-System
│
├── ambulance.ino
├── traffic.ino
├── images
│   ├── setup.jpg
│   ├── emergency-unit.jpg
│   ├── traffic-unit.jpg
│   ├── red-signal.jpg
│   └── green-signal.jpg
│
└── README.md
```

## Applications

* Smart Cities
* Intelligent Transportation Systems
* Emergency Vehicle Management
* Traffic Automation
* Urban Traffic Control
* Smart Road Infrastructure

## Future Improvements

* AI-based siren recognition
* GPS-based ambulance tracking
* Cloud monitoring dashboard
* Multiple traffic junction control
* Mobile application integration
* Real-time traffic analytics

## Project Images

### Complete Setup

Add the complete hardware setup image here.

### Emergency Vehicle Unit

Add the ESP32 and sound sensor image here.

### Traffic Signal Unit

Add the ESP32 traffic signal image here.

### Working Demonstration

Add images showing red, yellow, and green signal states.

## Author

N. I. Preetish

## License

This project is open-source and intended for educational and research purposes.
