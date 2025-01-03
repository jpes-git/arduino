# Freshwater Aquaculture Monitoring System

This project is an Internet of Things (IoT)-based system for monitoring and controlling freshwater aquaculture environments. It uses an ESP32 microcontroller to track environmental parameters such as temperature, pH levels, and dissolved oxygen, ensuring the optimal health of aquatic organisms. Notifications and automatic corrective actions are taken based on sensor readings.

## Features

1. **Temperature Monitoring**:
   - Real-time temperature readings in both Celsius and Fahrenheit.
   - Threshold-based email alerts for extreme temperatures.

2. **pH Monitoring**:
   - Monitors pH levels of water.
   - Sends email notifications when pH goes out of range.

3. **Dissolved Oxygen Monitoring**:
   - Tracks dissolved oxygen levels to ensure aeration needs.

4. **Automated Aeration**:
   - Automatically turns on/off the aerator based on temperature and oxygen levels.

5. **IoT Integration**:
   - Enables cloud connectivity for remote monitoring and control.

6. **Email Notifications**:
   - Alerts users via email when critical conditions occur.

## Components Used

- ESP32 Microcontroller
- DS18B20 Temperature Sensor
- pH Sensor
- Dissolved Oxygen Sensor
- Servo Motor for Feeder
- Relay Module
- WiFi for IoT Communication

## Prerequisites

- **Hardware**:
  - ESP32
  - Sensors: DS18B20, pH probe, DO sensor
  - Supporting components: Servo, relay, power supply

- **Software**:
  - Arduino IDE
  - Arduino IoT Cloud

## Installation

1. **Hardware Setup**:
   - Connect sensors and actuators as per your project schematic.

2. **Software Setup**:
   - Install the required Arduino libraries:
     - OneWire
     - DallasTemperature
     - ESP32Servo
     - ESP32_MailClient
   - Configure your WiFi credentials and update the sender/receiver email addresses in the code.

3. **Upload Code**:
   - Open the `.ino` file in Arduino IDE.
   - Select the correct board (ESP32) and COM port.
   - Upload the sketch to the ESP32.

## Usage

1. Power on the system and ensure all connections are secure.
2. Monitor real-time environmental parameters via the Arduino IoT Cloud dashboard.
3. Receive email notifications when values exceed predefined thresholds.
4. Adjust parameters such as threshold values directly through the IoT dashboard.

## File Structure

- `src/`
  - Contains the Arduino `.ino` source file for the project.
- `README.md`
  - Overview and instructions for the project.

## Author

Developed by John Patrick Salvatin, a graduate of Bachelor of Science in Computer Engineering. This project was part of the research titled **"Freshwater Aquaculture Monitoring and Control System Using ESP32 Microcontroller."**

## License

This project is open-source and available under the MIT License.
