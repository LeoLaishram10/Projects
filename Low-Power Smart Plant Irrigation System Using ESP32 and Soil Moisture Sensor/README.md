The Low-Power Smart Plant Irrigation System is an embedded IoT solution designed to automate plant watering while minimizing energy consumption. The system utilizes an ESP32 microcontroller, a capacitive soil moisture sensor, and a miniature DC water pump to monitor soil conditions and irrigate plants only when necessary.
The ESP32 periodically wakes from Deep Sleep mode to power the soil moisture sensor, acquire analog moisture data, and compare the measured value against a predefined threshold. If the soil is determined to be dry, the controller activates the water pump through a MOSFET driver for a fixed duration. After watering, the system rechecks the soil moisture to confirm adequate irrigation before returning to Deep Sleep.
To maximize battery life, both the ESP32 and soil moisture sensor employ aggressive power-saving techniques. The ESP32 remains asleep for most of its operating time, while the moisture sensor is powered only during sampling. These strategies significantly reduce average current consumption, making the system suitable for long-term battery-powered operation.
The project demonstrates practical implementation of embedded control systems, analog sensor interfacing, GPIO programming, ADC acquisition, low-power firmware design, and autonomous irrigation. It provides an economical, scalable, and environmentally friendly solution for smart agriculture and home gardening applications.

Hardware Used:
ESP32 Development Board
Soil Moisture Sensor
Mini DC Water Pump
IRLZ44N-mosfet
Flyback Diode-1N4007
two 18650 Lithium-Ion Battery in series
LM2596- step ddown buck converter to 3.3v
