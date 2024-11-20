# Iot-Based-health-tracker
This code is designed to monitor a user's heart rate and oxygen saturation level (SpO2) using a MAX30100 Pulse Oximeter sensor and transmit the readings to the Blynk IoT platform via an ESP8266 module. The setup enables real-time health monitoring and visualization through the Blynk app or dashboard.

Key features:

Wi-Fi Connectivity:

Connects to a Wi-Fi network using the credentials provided (ssid and pass).
Uses the Blynk platform for IoT connectivity, where the BLYNK_AUTH_TOKEN authenticates the device.
Sensor Integration:

Interfaces with the MAX30100 Pulse Oximeter sensor to measure:
Heart Rate (in beats per minute, bpm).
Oxygen Saturation (SpO2) (percentage of oxygen in the blood).
Includes a callback function (onBeatDetected) to detect individual heartbeats and log them to the serial monitor.
Data Reporting:

Reads and processes sensor data every second (REPORTING_PERIOD_MS = 1000 ms).
Outputs the readings to the Serial Monitor for debugging or local observation.
Sends the heart rate and SpO2 data to Blynk Virtual Pins (V1 and V2) for remote monitoring.
Error Handling:

Checks the initialization status of the MAX30100 sensor and logs an error message if it fails to initialize.
Real-Time Health Monitoring:

Designed for real-time remote health tracking, making it suitable for applications such as personal health devices or patient monitoring systems.

