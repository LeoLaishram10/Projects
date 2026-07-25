The Smartphone-Controlled Wi-Fi RC car is an embedded systems project that demonstrates wireless robotic control using the ESP8266 Wi-Fi microcontroller and the RemoteXY mobile application. The system enables a user to remotely navigate a robotic vehicle in real time through a smartphone by connecting directly to the ESP8266's Wi-Fi access point. The RemoteXY application provides an intuitive virtual joystick interface that transmits movement commands wirelessly without requiring an external Wi-Fi router or internet connection.
The ESP8266 processes joystick commands received from the RemoteXY application and generates differential motor control signals for the TB6612FNG dual H-Bridge motor driver, enabling forward, reverse, left, right, and pivot steering. Motor speed is regulated using Pulse Width Modulation (PWM) to achieve smooth and responsive movement.
The robotic vehicle is powered using two 18650 lithium-ion batteries, while an LM2596 buck converter provides a stable regulated supply voltage to the ESP8266, ensuring reliable wireless communication and preventing voltage fluctuations caused by motor load variations.
The project demonstrates the integration of embedded firmware development, wireless communication, motor control, voltage regulation, and real-time robotic systems, providing a practical foundation for mobile robotics and IoT-based automation applications.

Objectives:
> Design and develop a smartphone-controlled robotic vehicle using the ESP8266 Wi-Fi microcontroller.
> Implement wireless communication between the smartphone and the ESP8266 using the RemoteXY mobile application.
> Develop embedded firmware to process joystick commands received from RemoteXY.
> Implement differential drive steering using the TB6612FNG dual H-Bridge motor driver.
> Control motor speed using PWM for smooth vehicle operation.
> Design a stable power distribution system using the LM2596 buck converter.
> Integrate hardware and software for reliable real-time wireless control.

Hardware Components:
ESP8266 Development Board
TB6612FNG Dual H-Bridge Motor Driver
LM2596 Buck Converter
Two DC Geared Motors
Two 18650 Lithium-Ion Batteries
Chassis and Wheels
Smartphone with RemoteXY Application
Connecting Wires
