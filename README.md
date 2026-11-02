# ESP32 LED Blinking Using ESP-IDF

## Project Description
This is my first embedded systems project using the ESP32 microcontroller and ESP-IDF framework.

The project demonstrates how to configure a GPIO pin as an output and control an LED using Embedded C.

The LED turns ON for one second and OFF for one second continuously.

## Components Used
- ESP32-WROOM-32
- Red LED
- 330-ohm resistor
- Breadboard
- Jumper wires
- USB cable

## Software Used
- Xubuntu Linux
- ESP-IDF
- Visual Studio Code
- Wokwi Simulator
- Git

## GPIO Connections

| Component | ESP32 Pin |
|---|---|
| LED Anode (+) | GPIO 2 through 330-ohm resistor |
| LED Cathode (-) | GND |

## Concepts Learned
- GPIO configuration
- Digital output control
- Embedded C programming
- ESP-IDF project structure
- FreeRTOS delay functions
- Firmware compilation and building

## How It Works
1. Configure GPIO 2 as an output.
2. Set GPIO 2 HIGH to turn ON the LED.
3. Wait for one second.
4. Set GPIO 2 LOW to turn OFF the LED.
5. Wait for one second.
6. Repeat continuously.

## Build Instructions

Activate the ESP-IDF environment:

```bash
. ~/esp/esp-idf/export.sh
```

Set the ESP32 target:

```bash
idf.py set-target esp32
```

Build the project:

```bash
idf.py build
```

## Testing
- Firmware successfully built using ESP-IDF.
- LED blinking successfully tested using Wokwi simulation.
- Physical ESP32 hardware testing is pending.

## Future Improvements
- Push-button-controlled LED
- LED brightness control using PWM
- GPIO interrupt-based LED control
- Timer-based LED blinking

## Author
Embedded Systems Learner