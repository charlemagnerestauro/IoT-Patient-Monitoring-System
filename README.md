# IoT-Patient-Monitoring-System
ESP32-based IoT patient monitoring prototype with sensor measurements, OLED display, Blynk dashboard, and alert notifications.


# IoT-Based Patient Monitoring System

An ESP32-based IoT patient monitoring prototype designed to measure heart rate, blood oxygen saturation (SpO₂), body temperature, room temperature, and humidity.

The system displays sensor readings on an OLED screen and uses the Blynk IoT platform for remote monitoring and alert notifications.

## Features

- Heart rate and SpO₂ monitoring using MAX30100
- Body temperature measurement using DS18B20
- Room temperature and humidity monitoring using DHT22
- Local monitoring through a 0.96-inch OLED display
- Remote monitoring using Blynk IoT
- LED and buzzer alerts for predefined thresholds
- Sensor reading averaging and offline operation

## Hardware Components

| Component | Purpose |
|---|---|
| ESP32 Development Board | Main microcontroller |
| MAX30100 | Heart rate and SpO₂ sensor |
| DS18B20 | Temperature sensor |
| DHT22 | Temperature and humidity sensor |
| 0.96-inch OLED | Local display |
| Active Buzzer | Audible alerts |
| LED | Visual alerts |
| Resistors | Circuit connections and protection |

## Software and Libraries

- Arduino IDE
- Blynk IoT
- MAX30100_PulseOximeter
- DHT
- OneWire
- DallasTemperature
- Adafruit_GFX
- Adafruit_SSD1306

## Circuit Diagram

See the `hardware` folder for the circuit diagram and wiring schematic.

## System Flowchart

See the `docs` folder for the system operation flowchart.

## Getting Started

1. Install the Arduino IDE and configure the ESP32 board support.
2. Install the required libraries.
3. Connect the sensors, OLED, LED, and buzzer according to the circuit diagram.
4. Create a Blynk template and configure datastreams V1–V5 for the sensor readings.
5. Configure the Blynk dashboard and alert events.
6. Set your own Wi-Fi credentials and Blynk authentication token locally in the source code.
7. Upload the Arduino sketch to the ESP32.
8. Open the Serial Monitor and verify the sensor readings and Blynk connection.

## Project Status

Previous academic prototype. Hardware operation and measurement accuracy are not independently verified in this documentation.

## Disclaimer

This is an educational electronics project and is not intended for clinical monitoring, medical diagnosis, or emergency use.
