# RFID Door Access Control System

## Overview
This project implements a secure RFID-based door access system using Arduino and MFRC522 RFID reader.

## Hardware Used
- Arduino Uno
- MFRC522 RFID Reader
- Servo Motor (SG90 / MG90S)
- Buzzer Module
- RGY LED Module
- RTC DS1307
- External 5V Supply

## Software & Libraries
- Arduino IDE
- MFRC522 (Miguel Balboa)
- RTClib (Adafruit)
- Servo Library

## Step-by-Step Working
1. Wire the RFID module (3.3V only).
2. Upload `MASTER_DEBUG_RFID.ino` to verify communication.
3. Read card UID using `RFID_READ_NEW_CARD.ino`.
4. Replace UID in `VERIFIED_REGISTERED_RFID.ino`.
5. Upload final code and test access.

## Expected Output
- Authorized card → Green LED, servo unlock, short beep
- Unauthorized card → Red LED, alarm, access denied

## Safety Notes
- Never power MFRC522 with 5V
- Use external 5V for servo
- Common ground is mandatory

## Author
Arthansh Maurya
