# iot-distance-measurement

## Description

This repository hosts a Node.js project that combines Node-RED, an ESP32 microcontroller, MongoDB, and MQTT protocol for distance measurement using a distance sensor. The project incorporates the Moving Average algorithm and Weighted Moving Average algorithm for data processing and storage.

## Features

- Distance Measurement: The ESP32 microcontroller interfaces with the distance sensor to accurately measure distances.
- Node-RED Integration: Node-RED, a visual programming tool, is utilized for creating the flow, handling data processing, and MQTT communication.
- Moving Average Algorithm: The collected distance data is processed using the Moving Average algorithm, resulting in a smoothed and more stable output.
- Weighted Moving Average Algorithm: The Weighted Moving Average algorithm assigns varying weights to recent and historical data points, allowing for a focus on recent measurements.
- MongoDB Integration: MongoDB, a NoSQL database, is employed to store and manage the distance measurement data.
- MQTT Protocol: MQTT (Message Queuing Telemetry Transport) protocol is implemented for efficient and lightweight communication between the ESP32, Node-RED, and other MQTT-enabled devices.

## Dependencies

- Arduino IDE: The Arduino IDE is required to program the ESP32 microcontroller.
- ESP32 Board Library: The ESP32 board library must be installed in the Arduino IDE for programming the microcontroller.
- Node.js: Node.js is needed to run the Node-RED application and handle server-side operations.
- MongoDB: MongoDB must be installed and configured as the database management system.
- MQTT Broker: An MQTT broker, such as Mosquitto or Aedes, should be set up to facilitate MQTT communication.

## Installation

1. Connect the ESP32 microcontroller to your computer and open the Arduino IDE.
2. Install the ESP32 board library in the Arduino IDE.
3. Upload the provided Arduino sketch from the repository to the ESP32 microcontroller.
4. Install Node.js on your computer if not already installed.
5. Install Node-RED globally by executing the command `npm install -g node-red`.
6. Clone the repository to your local machine.
7. Navigate to the project directory and run `npm install` to install the required Node.js dependencies.
8. Set up and configure MongoDB as the database management system.
9. Install and configure an MQTT broker, such as Mosquitto or Aedes, for MQTT communication.
10. Import the file import-project.json to the Node-RED flow.
## Usage

1. Connect the distance sensor to the ESP32 microcontroller based on the provided circuit diagram.
2. Power on the ESP32 and ensure it is connected to your computer.
3. Launch Node-RED by executing the command `node-red` in your terminal.
4. Open a web browser and access the Node-RED interface at `http://localhost:1880`.
5. Import the provided Node-RED flow from the repository into your Node-RED workspace.
6. Deploy the flow and start collecting distance data.
7. The data will be processed using the Moving Average and Weighted Moving Average algorithms within the Node-RED flow.
8. The processed data will be stored in MongoDB for persistence and you able to query data at any time.
9. MQTT communication can be utilized for real-time data streaming and integration with other MQTT-enabled devices.

## Contributing

Contributions to this project are welcome. If you wish to contribute, please adhere to the standard guidelines for contributing, such as creating a new branch, making changes, and submitting a pull request. Ensure that your code aligns with the project's coding conventions and undergoes thorough testing.
