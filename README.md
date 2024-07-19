Project Note: ESP8266 Environmental Monitoring and LED Control using ThingSpeak
Project Overview
This project involves using an ESP8266 microcontroller to monitor environmental parameters such as temperature, humidity, and light intensity. The data is read from a DHT11 sensor and an LDR sensor, sent to a ThingSpeak channel, and LEDs are controlled based on the received data. The ESP8266 connects to a WiFi network, communicates with ThingSpeak to log sensor data, and retrieves data to make decisions for LED control.

Components Required
ESP8266 (e.g., NodeMCU)
DHT11 Sensor (for temperature and humidity)
LDR Sensor (for light intensity)
LEDs (3 LEDs for different indications)
Resistors (appropriate values for sensors and LEDs)
Breadboard and Jumper Wires
Power Supply (e.g., USB cable)


Libraries Used
ESP8266WiFi.h: Enables WiFi functionality on the ESP8266.
WiFiClient.h: Provides the client functionality for WiFi connections.
ThingSpeak.h: Enables interaction with the ThingSpeak API.
DHT.h: Enables interaction with the DHT11 sensor.



Circuit Diagram
DHT11 Sensor: Connect the data pin to D2, VCC to 3.3V, and GND to GND.
LDR Sensor: Connect one end to the 3.3V pin and the other end to the A0 (analog input) pin with a pull-down resistor to GND.
LEDs: Connect the positive legs (anodes) of the LEDs to D6, D7, and D8 through current-limiting resistors, and the negative legs (cathodes) to GND.
