# RFID Door Access Control System (RC522 + Arduino)

A complete RFID-based door access system using Arduino Uno, MFRC522 RFID reader,
servo motor, buzzer, RGB LED, and DS1307 RTC.

This repository is designed for:
- Beginners
- Juniors learning embedded systems
- RFID access control demonstrations

---

## Features
- RFID card authentication
- Authorized / Unauthorized access handling
- Servo-based door lock mechanism
- Audio-visual feedback (buzzer + RGB LED)
- Date & time logging using RTC
- Modular test and debug sketches

---

## Hardware Used
- Arduino Uno
- MFRC522 RFID Reader (SPI)
- Servo Motor (SG90 / MG90S)
- Buzzer Module (Active)
- RGB / RGY LED Module
- RTC DS1307
- External 5V supply for servo

---

## Repository Structure
| Folder | Purpose |
|---|---|
| `firmware/` | Arduino sketches |
| `hardware/` | Wiring & pin documentation |
| `docs/` | Explanation & guides |
| `media/` | Images & wiring photos |

---

## Step-by-Step Workflow
1. Verify RFID hardware communication
2. Read RFID card UID
3. Register authorized UID
4. Run final access-control system

Each step has a dedicated sketch.

---

## Arduino Sketches
| Sketch | Purpose |
|---|---|
| `MASTER_DEBUG_RFID.ino` | Verify wiring & module |
| `RFID_READ_NEW_CARD.ino` | Read card UID |
| `VERIFIED_REGISTERED_RFID.ino` | Final access control |

---

## Libraries Required
- MFRC522 (Miguel Balboa)
- RTClib (Adafruit)
- Servo (Arduino)

---

## Serial Monitor
- Baud Rate: `9600`
- Displays UID, timestamp, and access result

---

## Safety Notes
- RC522 **MUST be powered from 3.3V**
- Servo must use **external 5V**
- Common GND between all modules is mandatory

---

## License
MIT License – free to use and modify.

---

## Author
Arthansh Maurya  
Electronics & Communication Engineering
