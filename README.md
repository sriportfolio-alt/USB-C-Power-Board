# USB-C 5V Power Supply Board

A compact USB Type-C power input board designed to provide a regulated 5V supply for embedded systems and development projects.

This project demonstrates USB-C power sink implementation, PCB design best practices, power protection circuitry, and hardware documentation using KiCad.

---

## Features

- USB Type-C power input
- USB-C sink implementation using CC pull-down resistors
- 5V output
- Resettable Polyfuse for over-current protection
- TVS diode for ESD protection
- Power status LED
- Test points for debugging
- 2-layer PCB
- Designed using KiCad

---

## Applications

- ESP32 Projects
- STM32 Development
- IoT Devices
- Embedded Systems
- Robotics
- Sensor Nodes
- Portable Electronics

---

## Specifications

| Parameter | Value |
|------------|---------|
| Input Connector | USB Type-C |
| Input Voltage | 5V |
| Output Voltage | 5V |
| Maximum Current | 1A |
| PCB Layers | 2 |
| PCB Thickness | 1.6 mm |

---

## Hardware Overview

USB-C Connector
↓
Polyfuse
↓
TVS Protection
↓
5V Output
↓
Power LED

CC1 and CC2 are connected to ground through 5.1kΩ pull-down resistors to identify the board as a USB-C power sink.

---

## Bill of Materials

| Component | Description |
|------------|-------------|
| USB-C Connector | USB Type-C Receptacle |
| Polyfuse | 1A Resettable Fuse |
| TVS Diode | USB ESD Protection |
| 330Ω | LED Current Limiting |
| 5.1kΩ ×2 | USB-C CC Pull-down |
| 10µF Capacitor | Input Filtering |
| 100nF Capacitor | Decoupling |

---

## Design Considerations

- USB Type-C implemented according to USB-C sink requirements.
- 5.1kΩ pull-down resistors used on CC1 and CC2.
- Polyfuse protects against excessive current.
- TVS diode provides ESD protection.
- Short power paths minimize voltage drop.
- Continuous ground plane improves EMC and reduces noise.

---

## Software

- KiCad 9
- Interactive Router
- 3D Viewer

---

## Future Improvements

- USB Power Delivery (PD) Support
- 3.3V LDO Output
- Current Measurement
- Reverse Polarity Protection
- Buck Converter
- USB Data Support
- Output Protection IC

---

## Learning Outcomes

This project demonstrates:

- USB Type-C Fundamentals
- PCB Design
- Schematic Capture
- Power Supply Design
- ESD Protection
- PCB Layout
- Manufacturing File Generation
- Design for Manufacturing (DFM)

---

## Author

**Sriram**

Embedded Systems | PCB Design | IoT | STM32 | ESP32

GitHub: https://github.com/sriportfolio-alt

LinkedIn: www.linkedin.com/in/sriram-ganesan-a1a171226

---

## License

This project is licensed under the MIT License.
