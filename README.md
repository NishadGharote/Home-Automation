# Home-Automation
This project demonstrates how to use an ESP32 microcontroller to control relays over Wi-Fi using HTTP GET requests. It sets up a web server that listens for commands to toggle relay states.

Introduction
This project utilizes an ESP32 microcontroller to create a web server that allows remote control of two relays (Relay1 and Relay2) via HTTP GET requests. The ESP32 connects to a Wi-Fi network and hosts a server on port 80. Clients can send specific URLs to control the relays.

Features
Allows remote control of two relays via Wi-Fi.
Supports toggling of relay states (ON and OFF) using HTTP GET requests.
Provides real-time feedback through the Serial Monitor for debugging.
Setup
Requirements
Arduino IDE with ESP32 board support.
ESP32 development board.
Two relays connected to GPIO pins (Relay1 on GPIO 22, Relay2 on GPIO 23).
Wi-Fi network credentials (ssid and password).
Installation
Clone or download the repository.
Open the project in Arduino IDE.
Install the required libraries (WiFi.h).
Update ssid and password in the code with your Wi-Fi credentials.
Upload the code to your ESP32 board.
Usage
Power up your ESP32 board and ensure it connects to the configured Wi-Fi network.
Open the Serial Monitor in Arduino IDE to monitor the connection status (115200 baud).
Use a web browser or HTTP client to send GET requests to control the relays:
To turn Relay1 ON: http://<ESP32_IP>/B11
To turn Relay1 OFF: http://<ESP32_IP>/B10
To turn Relay2 ON: http://<ESP32_IP>/B21
To turn Relay2 OFF: http://<ESP32_IP>/B20
Replace <ESP32_IP> with the actual IP address assigned to your ESP32 by your Wi-Fi network.

Additional Notes:
Security: Consider implementing security measures such as HTTPS and authentication if deploying in a production environment.
Error Handling: Improve error handling and robustness based on specific use cases and network condition.
This README.md file provides comprehensive information about your ESP32 WiFi Controlled Relay Server project, guiding users on setup, usage, and contributions effectively. Adjust details as per your specific project implementation and requirements.





