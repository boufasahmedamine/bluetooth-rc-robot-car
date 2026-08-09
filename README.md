# Bluetooth-Controlled Robotic Vehicle

An Arduino-based Bluetooth-controlled robotic vehicle developed as an undergraduate embedded systems project.

The vehicle uses an **ATmega328P-based Arduino**, an **L298N motor driver**, and an **HC-05/HC-06 Bluetooth module** to control a differential-drive platform from a mobile device.

## Overview

The project was developed as a practical exercise in embedded programming, serial communication, motor control, and basic robotics.

Commands are sent from a Bluetooth-enabled mobile device to the vehicle through a serial connection. The Arduino interprets these commands and controls the motors through the L298N motor driver.

The project was developed as an educational laboratory implementation and was based in part on existing reference designs and commonly used Arduino robotics hardware.

## Hardware

| Component                | Role                           |
| ------------------------ | ------------------------------ |
| Arduino Uno / ATmega328P | Main controller                |
| L298N                    | Dual H-bridge motor driver     |
| HC-05 / HC-06            | Bluetooth serial communication |
| DC gear motors           | Vehicle propulsion             |
| Battery pack             | Power source                   |
| Wheels & chassis         | Mechanical platform            |

## Control

The original firmware uses simple single-character commands transmitted over Bluetooth:

| Command | Action     |
| :-----: | ---------- |
|   `F`   | Forward    |
|   `B`   | Reverse    |
|   `L`   | Turn left  |
|   `R`   | Turn right |
|   `S`   | Stop       |

The exact control behavior depends on the firmware version and motor wiring used in the project.

## Firmware

The repository preserves the original Arduino firmware used for the project.

The code is intentionally kept alongside the project documentation rather than being presented as a production robotics framework. The repository may also contain later cleanup or improvements where appropriate, while keeping the original implementation identifiable.

## Project Context

This project was developed during my undergraduate engineering studies as a hands-on implementation of concepts including:

* Embedded C/C++ programming
* UART serial communication
* Bluetooth communication
* DC motor control
* H-bridge motor drivers
* Basic hardware/software integration

The project draws on established Arduino-based robotics designs and is presented here as part of my engineering portfolio.

## Repository Contents

```text
firmware/       Arduino firmware
docs/           Project documentation
```

Additional project material may be added as the repository is progressively documented.

## Status

This repository is a cleaned and documented presentation of an earlier undergraduate project. It is primarily intended for archival, educational, and portfolio purposes rather than as a production-ready robotics platform.

## License

The project is distributed under the **Custom Non-Commercial Portfolio License** included in this repository.

Third-party components, libraries, reference designs, and other materials remain subject to their respective licenses and terms.
