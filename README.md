# IoT-Based Biomedical Monitoring System

## Overview
This project is an IoT-based biomedical monitoring system that continuously measures key health parameters, including:
- Room Temperature
- Humidity
- Heart Rate (BPM)
- Blood Oxygen Level (SpO2)
- Body Temperature

The system is built using an ESP32 microcontroller and integrates multiple sensors to capture and display real-time data on a web-based interface.

## Hardware Components
- **ESP32** – Microcontroller for processing and communication
- **DHT11 Sensor** – Measures room temperature and humidity
- **MAX30100 Pulse Oximeter** – Measures heart rate (BPM) and SpO2 levels
- **DS18B20 Temperature Sensor** – Measures body temperature
- **Resistor (4.7kΩ)** – Required for DS18B20 sensor
- **Connecting Wires** – For circuit connections

## Circuit Diagram
Refer to the following circuit diagram in the hardware folder to assemble the hardware setup.

## Software Requirements
- **Arduino IDE**
- **ESP32 Board Package**
- **Required Libraries**:
  - `WiFi.h`
  - `WebServer.h`
  - `Wire.h`
  - `MAX30100_PulseOximeter.h`
  - `OneWire.h`
  - `DallasTemperature.h`
  - `DHT.h`

## Installation and Setup
1. Install the required libraries in the Arduino IDE.
2. Connect the hardware components as per the circuit diagram.
3. Update the `ssid` and `password` variables in the code with your WiFi credentials.
4. Upload the code to the ESP32 using Arduino IDE.
5. Once uploaded, open the Serial Monitor to get the ESP32's IP address.
6. Enter the IP address in a web browser to view the real-time sensor data.

## Features
- **Web Interface**: Displays real-time sensor readings in a structured format.
- **Automatic Data Update**: Uses AJAX to refresh sensor data without reloading the page.
- **Heartbeat Detection**: Alerts if BPM crosses a predefined threshold.
- **Remote Monitoring**: View patient vitals over a WiFi network.

## Web Interface
The web-based dashboard displays:
- Room Temperature (°C)
- Room Humidity (%)
- Heart Rate (BPM)
- SpO2 (%)
- Body Temperature (°C)

## Future Improvements
- Integration with cloud storage for historical data logging.
- Mobile app for remote access and notifications.
- Enhanced UI with better styling and graphs.



