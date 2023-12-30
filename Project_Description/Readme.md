# Weather Monitoring System

## Introduction
We are delighted to present the Weather Monitoring System, a solution designed to provide real-time weather data collection and remote monitoring capabilities. This report outlines the features, components, and benefits of our system.

## Features
- Real-time monitoring of:
  - Temperature and Humidity
  - Barometric Pressure
  - Rain Detection
  - Light Levels
- Data displayed on a clear LCD screen.
- Data securely published to the cloud for remote access.
- Compact and user-friendly design.

## Components
Our system includes the following key components:
- **ESP8266 NodeMCU:** The brain of the system, providing Wi-Fi connectivity and processing power.
- **DHT11 Sensor:** Measures temperature and humidity with precision.
- **BMP180 Sensor:** Provides accurate barometric pressure data.
- **Rain Sensor:** Detects rainfall and provides valuable weather information.
- **LDR (Light-Dependent Resistor):** Monitors light levels in the environment.
- **I2C LCD Display:** Presents collected data on a user-friendly display.

## Component Connections for Weather Monitoring System
1. **ESP8266 NodeMCU (WiFi Module):**
   - Connect it to your computer using a USB cable for programming and power.

2. **DHT11 Sensor (Temperature and Humidity):**
   - VCC (Power) -> 3.3V on NodeMCU
   - GND (Ground) -> GND on NodeMCU
   - Data Out -> D4 on NodeMCU

3. **BMP180 Sensor (Barometric Pressure):**
   - VCC (Power) -> 3.3V on NodeMCU
   - GND (Ground) -> GND on NodeMCU
   - SDA (Serial Data) -> D2 on NodeMCU
   - SCL (Serial Clock) -> D1 on NodeMCU

4. **Rain Sensor:**
   - VCC -> 3.3V on NodeMCU
   - GND -> GND on NodeMCU
   - Signal -> D5 on NodeMCU

5. **LDR (Light-Dependent Resistor):**
   - Connect LDR and resistor in series.
   - Connect the junction to an analog pin (e.g., A0) on the NodeMCU.

6. **I2C LCD Display:**
   - VCC -> 5V on NodeMCU
   - GND -> GND on NodeMCU
   - SDA -> D2 on NodeMCU
   - SCL -> D1 on NodeMCU

## Block Diagram
![MQTT drawio](https://github.com/suresh-gbu/Weather-Monitoring-System/assets/73007468/09fcc311-0379-477c-8640-b35129d456e2)


## Libraries Used in the Code
1. **ESP8266WiFi:** Used to connect the ESP8266 microcontroller to your Wi-Fi network.
2. **DHT:** Used for reading data from the DHT11 sensor.
3. **Adafruit_BMP085:** Used for the BMP180 sensor.
4. **Adafruit_MQTT and Adafruit_MQTT_Client:** Used for MQTT communication with Adafruit IO.
5. **Wire:** Used for I2C communication.
6. **LiquidCrystal_I2C:** Used for controlling the I2C-enabled LCD display.

## Benefits
- Stay informed about weather conditions in real-time.
- Remote access to data via the cloud ensures you can monitor the weather from anywhere.
- The user-friendly interface allows easy data interpretation.
- Compact design and straightforward setup make the system accessible for all users.

## Conclusion
Our Weather Monitoring System is a reliable, user-friendly, and efficient solution for staying informed about weather conditions. Whether for personal use, agricultural applications, or research, this system offers valuable real-time data at your fingertips.

For any inquiries or further details, please feel free to contact us.

**Contact us at:** campussolutions9@gmail.com

Thank You ….
