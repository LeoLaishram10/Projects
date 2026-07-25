Project Synopsis: Anti-Sleep Alarm and Alcohol Detection Based Engine Lock System

Objective & Problem Statement:
Road fatalities are heavily driven by driver fatigue (microsleep) and driving under the influence of alcohol. While luxury vehicles offer high-end driver-monitoring tech, economy vehicles lack affordable, integrated safety mechanisms.  The primary goal of this project is to develop a low-cost, automated, and retrofit-capable embedded safety system that continuously monitors driver alertness and breath alcohol levels to proactively prevent accidents.

System Architecture & Hardware Components:
The system is built around an Arduino Nano microcontroller (ATmega328P) and divided into three stages:
Input Stage (Sensors):MQ-3 Alcohol Gas Sensor: Positioned near the steering column to measure breath alcohol concentrations. 
Eye-Blink / IR Sensor (or Camera Module): Monitors eyelid movement and closure duration (although laptop camera is used in this project).
Processing Stage:Arduino Nano: Processes analog/digital inputs, executes threshold comparisons for alcohol, and runs a temporal timer for eye closure.  
Output Stage (Actuators & Indicators):5V Relay Module: Wired to the vehicle ignition/DC motor to cut power when alcohol is detected.  
                                                      Piezo Buzzer: Triggers an audible alert if eyes remain closed.  
                                                      Status LEDs: Yellow LED blinks for alcohol hazards; Red LED lights up for drowsiness. 
                                                      
Working Logic & Process Flow:
Initialization: System powers on and keeps the engine ignition relay closed (Active/Running state).  
Alcohol Check: If breath alcohol levels exceed the preset safety threshold, the system immediately de-energizes the relay (locking the engine) and flashes the Yellow LED.  
Drowsiness Check: If the driver’s eyes remain closed for more than 3 seconds, the system identifies a microsleep/fatigue event, turns on the Red LED, and sounds the Piezo Buzzer until the driver opens their eyes.  
