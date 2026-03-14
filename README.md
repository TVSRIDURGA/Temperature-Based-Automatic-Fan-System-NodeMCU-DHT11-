# Temperature-Based-Automatic-Fan-System-NodeMCU-DHT11-
🌡️ IoT Temperature & Humidity Monitoring with Automatic Fan Control

An IoT-based system that monitors temperature and humidity using a DHT11 sensor and automatically controls a fan using a relay module.
The system uses NodeMCU (ESP8266) to send real-time sensor data to the Blynk IoT platform, allowing remote monitoring through a dashboard.

🚀 Features

->Real-time temperature monitoring
->Real-time humidity monitoring
->Automatic fan control based on temperature
->Cloud-based monitoring using Blynk
->ESP8266 WiFi connectivity
->Serial monitoring for debugging


🛠️ Technologies Used

**Hardware**

1.NodeMCU (ESP8266)
2.DHT11 Temperature & Humidity Sensor
3.Relay Module
4.Fan(12V)
5.Breadboard(optional)
6.Jumper Wires
7.NodeMCU Micro-USB (Type-B) Cable

**Software**

1.Arduino IDE
Libraries used
->ESP8266WiFi.h
->BlynkSimpleEsp8266.h
->DHT.h

2.Blynk IoT Platform
Used to monitor and control IoT devices remotely by sending sensor data to a cloud dashboard through the internet. 🌐📱

⚙️ System Architecture
DHT11 Sensor → NodeMCU (ESP8266) → WiFi → Blynk Cloud → Dashboard
                                   ↓
                               Relay Module
                                   ↓
                                  Fan

🔌 Hardware Connections
| Component      | NodeMCU Pin |
| -------------- | ----------- |
| DHT11 Data Pin | D5          |
| Relay IN       | D2          | 
| VCC            | 3.3V / 5V   |
| GND            | GND         |


💻 How the System Works
1.The DHT11 sensor measures temperature and humidity.
2.NodeMCU reads the sensor data every 2 seconds.
3.The data is sent to the Blynk cloud platform via WiFi.
4.The Blynk dashboard displays real-time temperature and humidity.
5.If the temperature exceeds 30°C, the NodeMCU activates the relay.
5.The relay turns ON the fan automatically.
6.When the temperature drops below the threshold, the fan turns OFF.

📱 Blynk Setup
The Blynk platform is used to visualize sensor data.
Steps used in the project:

1.Created a template in Blynk Console with hardware set as ESP8266.
2.Added Datastream V1 for temperature.
3.Added Datastream V2 for humidity.
4.Generated Blynk Auth Token.
5.Added the token in the Arduino code.
6.Created dashboard widgets:
->Gauge widget for Temperature
->Gauge widget for Humidity
*This allows real-time monitoring of environmental conditions.

1️⃣ Blynk Dashboard Screenshot
The Blynk IoT platform allows monitoring sensor data from both desktop (web dashboard) and mobile application.
The screenshots below show real-time temperature and humidity values received from the NodeMCU device.

💻 Laptop Dashboard (Blynk Web Console)
This dashboard is accessed through the Blynk web console, where users can monitor temperature and humidity values from a laptop or desktop browser.
![image](https://github.com/TVSRIDURGA/Temperature-Based-Automatic-Fan-System-NodeMCU-DHT11-/blob/d3e0c1bed39987db9495024f4bbba8fa4b738301/Laptop%20Dashboard%20(Blynk%20Web%20Console)(SS).png)

📱 Mobile Dashboard ScreenShot 
This dashboard is accessed through the Blynk web console, where users can monitor temperature and humidity values from a mobile  phone





