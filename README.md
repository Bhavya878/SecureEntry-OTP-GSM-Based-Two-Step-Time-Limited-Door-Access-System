# SecureEntry OTP – GSM-Based Two-Step Time-Limited Door Access System

## Table of Contents
- Project Overview
- Objectives
- Block Diagram
- System Architecture
- Hardware Requirements
- Software Requirements
- Working Principle
- Features
- Repository Structure
- Applications
- Future Enhancements

## Project Overview

**SecureEntry OTP** is a GSM-based two-step authentication door access control system designed to provide secure and time-limited access to authorized users.

The system uses GSM communication to deliver a One-Time Password (OTP) to the registered mobile number. The user must enter the received OTP through a keypad to gain access to the door. The OTP is valid only for a limited period, providing an additional layer of security.

The system integrates an LCD display, keypad, GSM module, Real-Time Clock (RTC), EEPROM, and door control mechanism to provide reliable and controlled access.

## Objectives

- To develop a secure door access control system using Embedded C.
- To implement two-step authentication for door security.
- To generate and verify One-Time Passwords (OTP).
- To send OTPs to authorized users through GSM communication.
- To provide time-limited OTP validation using RTC.
- To prevent unauthorized access through password verification.
- To improve security and reliability in door access systems.

## Block Diagram

The system consists of a microcontroller interfaced with GSM, keypad, LCD, RTC, EEPROM, and door control components.

**Block Diagram Image:**

Add your block diagram image here after uploading it to the repository.

`![SecureEntry OTP Block Diagram](system_block_diagram.png)`

## System Architecture

The system architecture consists of the following modules:

1. **Microcontroller:** Controls the complete operation of the system and coordinates communication between different modules.
2. **GSM Module:** Sends OTP messages to the registered mobile number.
3. **Keypad:** Allows the user to enter the received OTP.
4. **LCD Display:** Displays system messages, OTP prompts, and access status.
5. **RTC Module:** Maintains time information and supports time-based OTP validation.
6. **EEPROM:** Provides non-volatile storage for required system data.
7. **Door Control Unit:** Controls door locking and unlocking based on authentication results.

## Hardware Requirements

| Component | Purpose |
|---|---|
| Microcontroller Board | Main control unit |
| GSM Module | OTP message communication |
| 4x4 Keypad | OTP input |
| LCD Display | User interaction |
| RTC Module | Time management |
| SPI EEPROM | Non-volatile data storage |
| Door Lock Mechanism | Door access control |
| Power Supply | System power |

## Software Requirements

| Software | Purpose |
|---|---|
| Embedded C | Programming |
| Keil µVision | Code development and compilation |
| Flash Magic | Microcontroller programming |
| Serial Communication | GSM communication |

## Working Principle

1. The system initializes the microcontroller and all interfaced peripherals.
2. When an access request is initiated, the system starts the authentication process.
3. An OTP is generated and sent to the registered mobile number through the GSM module.
4. The user receives the OTP and enters it using the keypad.
5. The microcontroller verifies the entered OTP.
6. The RTC is used to check the OTP validity period.
7. If the OTP is correct and within the valid time limit, access is granted and the door is unlocked.
8. If the OTP is incorrect or expired, access is denied and the door remains locked.
9. The LCD displays the corresponding authentication status.

## Features

- GSM-based OTP communication.
- Two-step authentication.
- Time-limited OTP validation.
- Keypad-based password entry.
- LCD-based user interaction.
- RTC-based time management.
- EEPROM data storage.
- Controlled door locking and unlocking.
- Protection against unauthorized access.

## Repository Structure

The repository contains Embedded C source files and header files organized according to their functionality.

| File | Description |
|---|---|
| `main.c` | Main application program |
| `gsm.c`, `gsm.h` | GSM communication |
| `otp.c`, `otp.h` | OTP-related operations |
| `Keypad.c`, `kpm.h` | Keypad interfacing |
| `lcd.c`, `lcd.h` | LCD interfacing |
| `rtc.c`, `rtc.h` | Real-Time Clock operations |
| `spi.c`, `spi.h` | SPI communication |
| `spi_eeprom.c`, `spi_eeprom.h` | EEPROM interfacing |
| `door.c`, `door.h` | Door control |
| `eint.c`, `eint.h` | External interrupt handling |
| `switch.c`, `switch.h` | Switch interfacing |
| `user.c`, `user.h` | User-related operations |
| `uart.c`, `uart.h` | UART communication |
| `defines.h`, `types.h` | Common definitions and data types |

## Applications

- Residential door security systems.
- Office access control systems.
- Restricted-area security.
- Laboratories and institutional access control.
- Electronic security systems.

## Future Enhancements

- Integration with IoT-based remote monitoring.
- Mobile application for access management.
- Biometric authentication.
- Access attempt logging and monitoring.
- Enhanced OTP generation and security mechanisms.

---

**Project Title:** SecureEntry OTP – GSM-Based Two-Step Time-Limited Door Access System

**Domain:** Embedded Systems

**Programming Language:** Embedded C

**Controller:** [Add your exact microcontroller model]

**Author:** Bhavya Palloli
