# SMART-LIGHT-CONTROL

*COMPANY*: CODTECH IT SOLUTIONS 

*NAME*: AKEPOGU SATHVIK RAJ 

*INTERN ID*: CT04DH122

*DOMAIN*: INTERNET OF THINGS

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH


## DESCRIPTION

Description:
This project illustrates a basic and practical Smart Light Control System with an Arduino UNO microcontroller and the Tinkercad Circuits simulation environment. The purpose of this system is to operate an LED light digitally via commands inputted through the Serial Monitor, emulating an intelligent automation system where lighting is controlled programmatically as opposed to manually.
The prototype is meant to react to input from the user through the Serial Monitor, where:
• Input '1' makes the LED ON
• Input '0' makes the LED OFF
This is a simple way of digital control to demonstrate that how smart home automation systems in recent times accept signals from apps, sensors, or IoT platforms to switch lights and other appliances on/off.

Components Used:
• Arduino UNO
• Light Bulb
• 220-ohm resistor (to restrict current to the LED)
• Serial Monitor (as the user input interface)

Working Principle:
The Arduino is coded with the Arduino IDE within Tinkercad. The sketch contains Serial.begin() to define serial communication and a loop that continuously looks for received data using Serial.available() and Serial.read(). 
Depending on the received input:
•the character is '1', Arduino runs digitalWrite(LED_PIN, HIGH) to turn the LED ON.
•the character is '0', it runs digitalWrite(LED_PIN, LOW) to turn the LED OFF.
This interaction mimics remote control using a command interface and illustrates the primary logic of intelligent control systems.
From this we can learn :
•	How microcontrollers work with digital input
•	Promoting real-time Arduino interaction through the Serial Monitor
•	Inserting conditional logic in embedded programming
•	Building and simulating circuits virtually in Tinkercad
•	Accurately using resistors to protect components

Applications :
Although this prototype employs a basic LED, it exemplifies the reasoning involved in commanding real-world devices such as home lighting systems, streetlights, or automated indicators. It lays the basis for sophisticated smart home systems, where user input might soon be substituted with mobile apps, sensors, or voice assistants.
This simulation is an excellent place to start for beginners to learn IoT and automation with Arduino, providing both hands-on learning and project-oriented application.

Overview of code :
•	The variable incomingChar is used to store the character received from the Serial Monitor.
•	In the setup() function:
Serial.begin(9600); initializes serial communication at a baud rate of 9600 bps.
pinMode(13, OUTPUT); configures pin 13 as an output for controlling the LED.
•	In the loop() function:
It checks if any data is available on the Serial Monitor using Serial.available().
Reads the input character using Serial.read().
If the input is '1', the LED is turned ON using digitalWrite(13, HIGH).
If the input is '0', the LED is turned OFF using digitalWrite(13, LOW).


## OUTPUT

When light is on (serial monitor : 1)

![Image](https://github.com/user-attachments/assets/6a23b4a0-52a5-4230-90f9-2162d4571c24)  

When light is off (serial monitor : 0)

![Image](https://github.com/user-attachments/assets/a62f74c6-c327-481d-9569-9169a091b7d8)



