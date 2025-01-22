# Arduino-RFID-LEDs-Buzzer
# RFID-Based Access Control System

## Components and Connections

### RFID Module (RC522) to Arduino:

| RFID Pin | Arduino Pin |
|----------|-------------|
| VCC      | 3.3V         |
| GND      | GND          |
| SDA      | D10 (SS)     |
| SCK      | D13 (SCK)    |
| MOSI     | D11 (MOSI)   |
| MISO     | D12 (MISO)   |
| RST      | D9 (RST)     |

---

### LEDs and Buzzer Connections:

| Component               | Arduino Pin | Function                         |
|-------------------------|-------------|---------------------------------|
| Default LED (Always ON)  | D3          | Indicates system readiness     |
| Grant LED (Green)        | D4          | Lights up for authorized card  |
| Deny LED (Red)           | D5          | Lights up for unauthorized card|
| Buzzer                   | D6          | Different sounds for access states |

---

### I2C LCD to Arduino Connections:

| LCD Pin | Arduino Pin |
|---------|-------------|
| VCC     | 5V          |
| GND     | GND         |
| SDA     | A4 (SDA)    |
| SCL     | A5 (SCL)    |

---

## Project Description

This project uses an **RFID module (RC522)** to create an access control system with Arduino. The system checks RFID tags against a stored authorized UID and provides visual and audio feedback based on access status.

## Features

- **Real-time access control** using RFID tags.
- **Visual feedback** with LEDs:
  - Default LED stays ON to indicate system readiness.
  - Green LED lights up for access granted.
  - Red LED lights up for access denied.
- **Audio feedback** with a buzzer for different access responses.
- **LCD Display (16x2)** to show user prompts and results.

## How to Use

1. Upload the Arduino code to your board.
2. Connect the components as described above.
3. Scan an RFID card to check access.
4. Observe LED and buzzer indications along with LCD messages.

---

## Example Output

### Authorized Card:

