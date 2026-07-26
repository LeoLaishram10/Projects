180° Ultrasonic Object Scanning System: An Arduino-based embedded system that performs real-time environmental scanning and obstacle detection using an ultrasonic distance sensor, a servo-driven sweeping mechanism, and a buzzer.

Project Detail:

This project implements a dynamic obstacle tracking radar using an Arduino Uno, an HC-SR04 Ultrasonic Sensor, and an SG90 Micro Servo Motor. The system continuously rotates the sensor across a semi-circular path to calculate object proximity. If an object enters a pre-configured safe zone, the system triggers an active audible alarm beep and alerts the user.
Key Features:
Automated 180° Environment Scanning: Smooth dual-sweep motor movement using PWM control.
Real-time Proximity Measurement: High-accuracy distance calculation derived from ultrasound pulse propagation times.
Non-Blocking Alarm Trigger: Instant audio alert via a piezoelectric buzzer when obstacles breach below 20cm threshold.
Serial Telemetry Stream: Outputs real-time telemetry (Angle, Distance) to the Arduino Serial Monitor at 9600 baud for logging and data visualization.

Hardware Components:
> Arduino Uno as the Main Microcontroller Board.
> SG90 Servo Motor as the 180 degree Directional Actuation.
> Piezo Buzzeras the Active Proximity Audio Warning.
