# SIGNAL-X
Portable ESP32-based RF signal capture, analysis, storage and controlled replay system.
# SIGNAL-X

### Portable RF Signal Capture, Analysis, Storage & Controlled Replay System

![Project Status](https://img.shields.io/badge/status-in%20development-orange)
![Platform](https://img.shields.io/badge/platform-ESP32-blue)
![License](https://img.shields.io/badge/license-MIT-green)

---

## Overview

SIGNAL-X is a portable embedded RF experimentation platform designed to
detect, capture, analyze, store and reproduce authorized test signals.

The system combines an ESP32 microcontroller with an RF receiver/transmitter,
display, local storage and physical controls to create a standalone signal
analysis and controlled replay device.

> This project is intended for experimentation with signals and equipment
> that we own or are explicitly authorized to test.

---

## Objectives

- Detect RF activity within the supported operating range
- Capture authorized test signals
- Analyze signal characteristics
- Store captured signal data locally
- Assign names to stored signals
- Recall previously stored signals
- Perform controlled signal replay
- Provide a standalone physical user interface
- Document the complete hardware and software development process

---

## System Architecture

```text
             ANTENNA
                |
                v
        +---------------+
        | RF FRONT END  |
        +-------+-------+
                |
                v
        +---------------+
        | RF RECEIVER   |
        +-------+-------+
                |
                v
        +---------------+
        |    ESP32      |
        | Processing    |
        | Control       |
        +---+-------+---+
            |       |
            v       v
        +------+  +------+
        | OLED |  |  SD  |
        | UI   |  | Card |
        +------+  +------+
            |
            v
       CONTROL INPUTS
            |
            v
       REPLAY ENGINE
            |
            v
       RF TRANSMITTER
Hardware
Component	Purpose
ESP32	Main controller
RF Receiver	Signal acquisition
RF Transmitter	Controlled replay
OLED Display	User interface
MicroSD Module	Signal storage
Rotary Encoder	Menu navigation
Push Buttons	User controls
Antennas	RF interface
Battery / Power System	Portable operation
Development Status
Stage	Status
Project architecture	🟢 Complete
Hardware selection	🟡 In progress
ESP32 firmware	⚪ Not started
RF capture	⚪ Not started
Signal analysis	⚪ Not started
Storage system	⚪ Not started
Replay system	⚪ Not started
Enclosure	⚪ Not started
Testing	⚪ Not started
Final documentation	⚪ Not started
