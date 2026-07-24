# SELF-DRIVING-FORK-LIFTER
An Arduino-based autonomous self driving robot with a servo-operated forklift mechanism. The robot follows a predefined path, detects and lifts an object, transports it to the destination, turns back, and follows the line to return to the starting point.

## Features

- Line following using dual IR sensors
- Automatic object detection
- Servo-controlled forklift mechanism
- DC motor control using L298N motor driver
- Automatic turn-back at the end of the path
- Return-to-start navigation
- Simple and efficient Arduino implementation

## Hardware Requirements

- Arduino Uno
- L298N Motor Driver
- 2 × DC Geared Motors
- 2 × IR Line Tracking Sensors
- IR Object Detection Sensor
- Servo Motor (SG90/MG90S)
- Robot Chassis
- Wheels
- Battery Pack
- Jumper Wires

## Pin Configuration

| Component | Arduino Pin |
|----------|-------------|
| Left Motor IN1 | D8 |
| Left Motor IN2 | D9 |
| Right Motor IN3 | D10 |
| Right Motor IN4 | D11 |
| Left Line Sensor | D4 |
| Right Line Sensor | D5 |
| IR Object Sensor | D2 |
| Servo Motor | D7 |

## Working Principle

1. The robot follows a black line using two IR line sensors.
2. When an object is detected, the IR object sensor triggers the servo to lift the object.
3. The robot continues following the path while carrying the object.
4. At the end of the route, the robot performs a turn-back maneuver.
5. The robot follows the same line back toward the starting point.
6. The servo can lower the object at the destination or starting position based on the program logic.

## Software

- Arduino IDE
- Servo Library (`Servo.h`)

## Project Structure

```
Line-Follower-Forklift-Robot/
│
├── Line_Follower_Forklift.ino
├── README.md
└── Images/
    ├── robot.jpg
    └── circuit_diagram.png
```

## Future Improvements

- PID-based line following for smoother navigation
- Automatic unloading mechanism
- Obstacle detection and avoidance
- Wireless monitoring using ESP32 or Bluetooth
- Battery voltage monitoring
- OLED/LCD status display

## Applications

- Warehouse automation
- Material handling
- Smart manufacturing
- Educational robotics
- Embedded systems learning

## Author

**Julius**

Engineering Student | Embedded Systems | Arduino | IoT | PCB Design

---

If you found this project helpful, consider giving it a ⭐ on GitHub!
