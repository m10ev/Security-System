# 🔐 Security-System

An **Arduino-based security system** that uses a **4x4 keypad** and **16x2 LCD screen** for user interaction. The system is designed to monitor multiple motion-sensitive sectors, allowing each to be armed/disarmed individually with sector-specific passwords, as well as a master password for full control.

## 🛠 Features

- Multi-sector security management (the 3 sectors can be expanded)
- Password-protected arming/disarming
- Individual passwords per sector
- Master password for system-wide control
- Alarm system with buzzer and LED indicator
- Disarm timeout with countdown
- Keypad input and LCD feedback
- Easily expandable and customizable

## 📷 System Schematics

### Thinkercad 
![Electronical Schematic](Media/Pictures/ElectronicalSchema.png)

### Electrical Schematic  
![Electrical Schematic](Media/Pictures/ElectricalSchema.png)

## ⚙️ Hardware Components

- Arduino UNO (or compatible board)
- 3 × PIR Motion Sensors
- 1 × 16x2 LCD Display (I2C or standard)
- 1 × 4x4 Keypad
- 1 × Buzzer
- 1 × LED
- Resistors, wires, breadboard (or PCB)

## 🧠 How It Works

1. On startup, user sets or confirms a master password.
2. The system allows selecting a sector using the keypad.
3. Each sector can be armed/disarmed with its own password.
4. If motion is detected in an armed sector:
   - A 15-second countdown begins.
   - User can disarm with the sector password.
   - If not, the system triggers an alarm.
5. The alarm can only be disabled with the master password.

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/m10ev/Security-System.git
