# Robot Dog PCB

This project is a custom **double-layer PCB** designed for a robot dog. The board is built around an **Arduino Nano** and provides connections for four servo motors, a battery input, a power switch, a DC-DC boost converter, an MPU6050 sensor, and an HC-SR04 ultrasonic sensor.

## Main Components

- Arduino Nano
- 4 × Servo motor connectors
- MPU6050 IMU sensor
- HC-SR04 ultrasonic sensor
- DC-DC boost converter
- ON/OFF switch
- Battery connector
- Double-layer PCB

## Features

- Controls four servo motors
- Uses the MPU6050 for motion and orientation sensing
- Uses the HC-SR04 for obstacle/distance detection
- Includes a battery power input
- Includes an ON/OFF switch
- Uses a DC-DC converter for regulated power
- Designed using both top and bottom copper layers

## Servo Connections

Each servo uses a 3-pin male header:

- Pin 1 → Signal
- Pin 2 → +5V
- Pin 3 → GND

## Sensors

### MPU6050
Connected to the Arduino using I2C:

- SDA → A4
- SCL → A5
- GND → GND
- 3.3V → 3.3V

### HC-SR04

- TRIG → Digital pin
- ECHO → Digital pin
- VCC → 5V
- GND → GND

## PCB Design

The PCB was designed in **EasyEDA** using two copper layers. Components were arranged to keep the board compact while keeping the servo and sensor connectors accessible.

## Screenshots

### Schematic
<img width="722" height="728" alt="Screenshot 2026-08-08 041312" src="https://github.com/user-attachments/assets/32fd3998-abc8-481b-92f0-7dac6b7a3231" />


### PCB Routing
<img width="761" height="470" alt="Screenshot 2026-08-08 041303" src="https://github.com/user-attachments/assets/65d1e148-9dc3-4fd6-a0ae-dfed5bc7cde1" />


### 3D View
<img width="1272" height="666" alt="Screenshot 2026-08-08 041248" src="https://github.com/user-attachments/assets/d39ca6ae-d11c-4323-b5d4-b8c2936dfd7b" />


## Design Check

The final PCB routing was checked using EasyEDA's **Design Rule Check (DRC)** to verify the connections and detect routing errors.
