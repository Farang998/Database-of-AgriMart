# Database-of-AgriMart
One-stop-Shop for all

# Environmental Monitoring System

This project focuses on building a real-time Environmental Monitoring System using ESP32 microcontrollers and various sensors. The system is capable of measuring and transmitting data such as temperature, humidity, pressure, current, and gas concentration.

## System Overview

The system uses two ESP32 boards configured in a master-slave architecture using the MODBUS RTU protocol. The slave ESP32 reads data from multiple sensors and sends it to the master ESP32. The master then publishes this data over MQTT to a Node.js server, which stores the data in a MongoDB database. A DWIN touch display is used to show the data visually.

## Components Used

- ESP32 (2 units)
- DHT22 (Temperature and Humidity Sensor)
- BMP280 (Pressure Sensor)
- ACS712 (Current Sensor)
- MQ135 (Gas Sensor)
- DWIN HDL662B Display
- SD card for DWIN display files

## Technologies

- Arduino IDE (ESP32 programming)
- MODBUS RTU protocol
- MQTT (via HiveMQ broker)
- Node.js (Express, Mongoose, MQTT)
- MongoDB
- DGUS Software (for DWIN display interface)
- HTML, CSS, JavaScript (for frontend display)

## Project Files

- `Final_Master.ino` – Code for master ESP32 (MODBUS read + MQTT publish)
- `Final_Slave.ino` – Code for slave ESP32 (sensor read + MODBUS write)
- `Project_Report.pdf` – Complete project documentation
- `Project_Poster.pdf` – Project poster for presentation

For more details on implementation and issues faced during development, refer to the report and code files.
