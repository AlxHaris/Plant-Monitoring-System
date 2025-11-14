# Plant-Monitoring-System
IoT-Based Plant Monitoring System
->**Project Overview**

The IoT-Based Plant Monitoring System helps monitor soil and environmental conditions in real time using IoT sensors.
It ensures that plants receive optimal care by measuring key parameters and alerting when action is needed.

**The system focuses on two main aspects:**

🌿 Soil Moisture – to determine when irrigation is required.
🌡️ Temperature & 💧 Humidity – to maintain suitable environmental conditions for plant growth.
The system uses Arduino for sensor data collection and Java for processing, monitoring, and alerting.
It demonstrates key Object-Oriented Programming (OOP) concepts such as classes, inheritance, encapsulation, and polymorphism.

**Hardware Used**
**Component**   ->	 **Function**
Arduino Uno  -> 	Microcontroller to read sensor data
DHT22 Sensor	-> Measures temperature and humidity
Soil Moisture -> Sensor	Detects water content in soil
USB Cable	For -> serial data communication
Jumper Wires	-> Connect sensors to Arduino

**How It Works**
**🪴 Sensors Collect Data**
Soil Moisture Sensor → Measures the amount of water in the soil.
DHT22 Sensor → Reads temperature and humidity from the environment.
Arduino reads the sensor values and sends them to the Java program via Serial communication (USB).

💻**Java Program Monitors the Farm**

The Java application receives real-time data from Arduino and performs the following:
If Soil Moisture < 30% → Displays an Irrigation Alert 💧
If Temperature > 30°C → Displays a High Temperature Alert 🌡️
If Humidity < 50% → Displays a Low Humidity Alert 💨
All readings and alerts are shown in the console and optionally saved in a file for analysis.

**OOP Concepts Used**
**Concept**	        -          **Example**
Encapsulation   -	Private variables with getters/setters in Sensor
Inheritance     -	SoilMoistureSensor and EnvironmentSensor extend Sensor
Polymorphism	  -  Overriding readData() method for each sensor type
Abstraction	     - Common Sensor class defines shared behavior

**🌟 Features**
✅ Real-time monitoring of soil and environmental parameters.
✅ Alerts for irrigation, temperature, and humidity conditions.
✅ Implements OOP principles in Java.
✅ Uses File Handling to save readings.
✅ Works with real Arduino sensors or simulated data.
✅ Expandable to include cloud storage or remote monitoring.

**System Flow**
[ DHT22 + Soil Sensor ]
          ↓
      [ Arduino UNO ]
          ↓ (Serial Communication)
       [ Java Program ]
          ↓
 [ Console Alerts + Data Logging ]


