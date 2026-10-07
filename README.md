# ESP32 Development Board

A custom **ESP32 development board** designed in **EasyEDA** for learning PCB design and embedded systems.

The board is based on the **ESP32-WROOM-32E** module and includes USB programming, voltage regulation, automatic boot/reset circuit, ESD protection, status LEDs, and GPIO headers for easy prototyping.

---

## Features

- ESP32-WROOM-32E (4MB Flash)
- CP2102N USB-to-UART
- AMS1117-3.3V regulator
- USB Micro connector
- BOOT & RESET buttons
- Power and User LEDs
- ESD protection
- Decoupling capacitors
- GPIO headers
- Designed in EasyEDA

---

## Hardware Specifications

| Item | Specification |
|------|---------------|
| MCU | ESP32-WROOM-32E |
| Flash | 4 MB |
| USB Interface | CP2102N |
| Input Voltage | 5V USB |
| Operating Voltage | 3.3V |
| Wireless | Wi-Fi + Bluetooth |
| Programming | USB |

---

# Images

## PCB

```
images/pcb.png
```

## 3D View

```
images/3d.png
```

## Schematic

```
images/schematic.png
```

---

# GPIO

The board exposes most ESP32 GPIO pins for development.

```
0 2 4 5
12 13 14 15
16 17 18 19
21 22 23
25 26 27
32 33 34 35
36 39
```

---

# Bill of Materials (BOM)

| Qty | Component | LCSC Part | Link |
|---:|-----------|-----------|------|
| 8 | 100nF Capacitor | C1525 | https://www.lcsc.com/product-detail/C1525.html |
| 2 | 22uF Capacitor | C602037 | https://www.lcsc.com/product-detail/C602037.html |
| 1 | 4.7uF Capacitor | C368809 | https://www.lcsc.com/product-detail/C368809.html |
| 2 | 10uF Capacitor | C315248 | https://www.lcsc.com/product-detail/C315248.html |
| 1 | 1×2 Pin Header | C2935942 | https://www.lcsc.com/product-detail/C2935942.html |
| 1 | 1×3 Pin Header | C124354 | https://www.lcsc.com/product-detail/C124354.html |
| 2 | SS8050 NPN | C3199946 | https://www.lcsc.com/product-detail/C3199946.html |
| 2 | 2N7002 MOSFET | C139445 | https://www.lcsc.com/product-detail/C139445.html |
| 2 | 1kΩ Resistor | C17513 | https://www.lcsc.com/product-detail/C17513.html |
| 5 | 10kΩ Resistor | C25744 | https://www.lcsc.com/product-detail/C25744.html |
| 2 | 10kΩ Resistor (0805) | C17414 | https://www.lcsc.com/product-detail/C17414.html |
| 2 | 0Ω Resistor | C17168 | https://www.lcsc.com/product-detail/C17168.html |
| 3 | 22.1kΩ Resistor | C43473 | https://www.lcsc.com/product-detail/C43473.html |
| 1 | 47.5kΩ Resistor | C325696 | https://www.lcsc.com/product-detail/C325696.html |
| 2 | Tactile Switch | C920224 | https://www.lcsc.com/product-detail/C920224.html |
| 1 | ESP32-WROOM-32E | C701341 | https://www.lcsc.com/product-detail/C701341.html |
| 1 | CP2102N | C1550553 | https://www.lcsc.com/product-detail/C1550553.html |
| 1 | AMS1117-3.3 | C347222 | https://www.lcsc.com/product-detail/C347222.html |
| 3 | ESD Diode | C7433850 | https://www.lcsc.com/product-detail/C7433850.html |
| 2 | 0805 LED | C6679547 | https://www.lcsc.com/product-detail/C6679547.html |
| 2 | 17 Pin Header | C5243697 | https://www.lcsc.com/product-detail/C5243697.html |
| 1 | Micro USB Connector | C136000 | https://www.lcsc.com/product-detail/C136000.html |

---

# Assembly Tools

- Soldering iron
- Solder wire
- Flux
- Tweezers
- USB cable
- Multimeter

---

# Arduino IDE

Install:

- ESP32 Board Package
- CP210x Driver

Select:

```
Board: ESP32 Dev Module
```

---

# Example

```cpp
#define LED_PIN 2

void setup() {
  pinMode(LED_PIN, OUTPUT);
}

void loop() {
  digitalWrite(LED_PIN, HIGH);
  delay(500);
  digitalWrite(LED_PIN, LOW);
  delay(500);
}
```

---



---

# What I Learned

- ESP32 hardware design
- USB to UART circuit
- Power supply design
- PCB routing
- Decoupling capacitor placement
- ESD protection
- PCB antenna keep-out
- PCB manufacturing workflow

---

# License

MIT License

---

# Credits

Designed and developed by **Sugam Pathak**

Created as a learning project using **EasyEDA**.
