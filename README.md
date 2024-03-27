# Assignment_3
IoT Assignment 3. Spring 2024 
# Environmental Sensor Data Publisher to ThingSpeak

## Overview
This project is designed to collect environmental data, specifically temperature, humidity, and CO2 levels, and publish it to ThingSpeak using MQTT. The project uses a microcontroller (not specified) with networking capabilities to connect to the internet via Wi-Fi and publish sensor data at regular intervals.

## Features
- **Data Collection:** Randomly generates environmental data (temperature, humidity, CO2) for demonstration purposes.
- **MQTT Integration:** Utilizes MQTT protocol to securely and efficiently publish data to the ThingSpeak platform.
- **Wi-Fi Connectivity:** Connects to a Wi-Fi network for internet access.
- **Continuous Monitoring:** Designed to run continuously, publishing data at 10-second intervals.

## Hardware Requirements
- A microcontroller with Wi-Fi and networking capabilities (e.g., ESP8266, ESP32).
- (Optional) Actual environmental sensors for temperature, humidity, and CO2, if real data collection is desired.

## Software Dependencies
- `network` module for Wi-Fi connectivity.
- `umqtt.simple` for MQTT communication.
- `urandom` for generating random data (for testing purposes).

## Setup and Configuration
1. Replace `WIFI_SSID` and `WIFI_PASSWORD` with your Wi-Fi network's details.
2. Update `mqtt_client_id`, `mqtt_user`, `mqtt_password`, `mqtt_server`, and `mqtt_topic_*` with your ThingSpeak MQTT credentials and topic information.
3. Deploy the code to your microcontroller.

## Usage
Once set up, the device will automatically connect to Wi-Fi, generate sensor data, and publish it to the specified ThingSpeak channel fields at 10-second intervals.


