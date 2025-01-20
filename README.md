# MECHATRONICS-GROUP-2-ROBOTICS-PROJECT-OBSTACLE-AVOIDANCE-
 
 DESIGN AND IMPLEMENTATION OF OBSTACLE AVOIDANCE ROBOT USING ARDUINO UNO R3

LEVEL 200 FIRST SEMESTER PROJECT

BY

MECHATRONICS ROBOTICS GROUP 2

BELLS UNIVERSITY OF TECHNOLOGY, OTA (BUT)
DEPARTMENT OF MECHATRONICS ENGINEERING

JANUARY, 3TH, 2025

# DECLARATION

I hereby declare that this is our original work of the project design reflecting the knowledge acquired from research on my level 200 1st semester project about “Design and implementation of obstacle avoidance robot using Arduino UNO R3”, I therefore declare that the information in this report is original and has never been submitted to any other institution, university or college for any award other than Bells University of Technology, Department of Mechatronics Engineering, Ota.

S/N	SURNAME	NAME	MATRIC NUMBER	DEPARTMENT	SIGNATURE
1.	ADENIYI	EXCEL	2023/12664	MECHATRONICS	
2.	ADETUNJI	JOSHUA	2023/12683	MECHATRONICS	
3.	ADEWOLE	MUBARAK	2023/12582	MECHATRONICS	
4.	ADELEKE	OLUWAFERANMI	2023/12245	MECHATRONICS	
5.	ADESINA	EMMANUEL	2023/12416	MECHATRONICS	
THE SIGNATURES HERE ARE FOR THE MEMBERS WHO PARTICIPATED IN THE PROJECT

# APPROVAL

I have read and hereby recommended this final year project design entitled “Design and implementation of obstacle avoidance robot using Arduino UNO R3” acceptance of Bells University of Technology in the fulfilment for the requirement of the level 200 1st semester robotics project in Mechatronics Engineering.

…………………………………………..
Ayuba Muhammad
Lecturer


# ACKNOWLEDGEMENT

I would like to thank my group members for being co-operative, I would also like to thank Olaniyi Oluwatobiloba who helped in a minor error with the ultrasonic sensor trigger and echo pin while coding the Arduino UNO R3 board.


# DEDICATION

I dedicate this project to LORD almighty for the strength and knowledge he gave group two to complete this project. I also dedicate this project to myself, Adeniyi Excel. And I also dedicate this project to Trex AI for it’s help in debugging my code.


# TABLE OF CONTENTS 

Declaration
Approval
Acknowledgement
Dedication
List of Figures
Abstract

CHAPTER ONE
	Introduction
	Background of the Study
	Problem Statement
Objectives of the Study
•	Main objectives
•	Specific objectives
•	Research question
Significance of the Study
Scope of Study
•	Context Scope
•	Geographical Scope
•	Time Scope
CHAPTER TWO
Introduction Ultrasonic Sensor
•	Components
•	Principle of Ultrasonic Sensor
•	Advantages
•	Application In a Vacuum Cleaning Robot
•	Limitation
Related work done

CHAPTER THREE
	System Components
	Design of System
•	System Functionality
•	Functionality of The Design
	Working of The System

CHAPTER FOUR
	System Code
•	Function of the code
Result of The System

CHAPTER FIVE
	Conclusion
	Recommendation
REFECENCES



# LIST OF FIGURES

Fig 1: Ultrasonic Sensor Principle
Fig 2: Principle of an ultrasonic sensor
Fig 3: Schematic of the System
Fig 4: Components of the System
Fig 5: Arduino Uno R3 Board
Fig 6: LCD 16x2
Fig 7: LED (Yellow)
Fig 8: DC Motor
Fig 9: H-Bridge Motor Driver
Fig 10: Ultrasonic Sensor
Fig 11: Resistor
Fig 12: Proteus Simulation of the System
Fig 13: LCD Running Simulation
Fig 14: Preview of the Code


# ABSTRACT

In the current times, automated house hold appliances have become a popular choice for house hold cleaning agents such has a vacuum bot but there have been lots of report about robots accidentally hitting an obstacle thereby damaging the robot and causing the robot’s inability to complete its task. A common household would feel much at ease if the vacuum bots avoid every obstacle in its way and efficiently clean the house. Hence this project is a prototype of an obstacle avoiding system that can be implemented in house hold cleaning robots for minimal cost.
Index-Terms: Arduino UNO R3, LED, motors, LCD 16x2, ultrasonic sensor, channel driver with diodes.


# CHAPTER ONE
INTRODUCTION 

The advent of automated household appliances has revolutionized the way we maintain our homes. Robots like vacuum bots have become increasingly popular, offering unparalleled convenience and efficiency in cleaning tasks. These robots have transformed the cleaning landscape, enabling homeowners to allocate more time to leisure activities and less time to mundane chores. However, their usefulness is often hindered by a significant limitation: the inability to detect and avoid obstacles.

Numerous reports have highlighted the frequency of collisions, resulting in damage to the robot and incomplete cleaning tasks. This not only leads to additional maintenance costs but also compromises the overall cleaning experience. Furthermore, the risk of accidents and injuries posed by these collisions underscores the need for a reliable obstacle avoidance system.

To address this challenge, this project focuses on designing and developing a prototype obstacle avoidance system. This innovative solution aims to enable household cleaning robots to efficiently navigate around obstacles, ensuring comprehensive and damage-free cleaning operations. By leveraging affordable components, including Arduino UNO R3, LEDs, motors, LCD 16x2, ultrasonic sensors, and channel drivers with diodes, this system promises to enhance the reliability and effectiveness of household cleaning robots.

The successful implementation of this obstacle avoidance system will have far-reaching implications for the future of household cleaning robots. Homeowners will benefit from increased efficiency, reduced maintenance costs, and enhanced safety. Moreover, this technology will pave the way for the development of more sophisticated and autonomous cleaning solutions, transforming the cleaning landscape forever.

This project seeks to contribute to the growing field of robotics and artificial intelligence, pushing the boundaries of innovation and excellence. Through the design and development of this obstacle avoidance system, we aim to make a meaningful impact on the daily lives of people, providing them with more time, convenience, and peace of mind.


BACKGROUND OF THE STUDY
The increasing demand for automated household appliances has led to the development of various robotic cleaning systems. Among these, vacuum cleaning robots have gained significant popularity due to their ability to efficiently navigate and clean floors. However, despite their advantages, these robots often struggle with obstacle detection and avoidance, resulting in collisions, damage, and incomplete cleaning tasks.

This project aims to develop a more efficient and effective obstacle avoidance system for vacuum cleaning robots. The proposed system utilizes a combination of ultrasonic sensors and Arduino UNO R3 microcontroller to detect and respond to obstacles.

The system operates by emitting high-frequency ultrasonic waves and detecting the echoes that bounce back from nearby objects. The Arduino UNO R3 microcontroller processes the sensor data and calculates the distance and location of obstacles. Based on this information, the system adjusts the robot's navigation path in real-time to avoid collisions.
The proposed system offers several advantages over current systems. Firstly, ultrasonic sensors are less affected by environmental factors and provide more accurate distance measurements. Secondly, the system's ability to detect and respond to obstacles in real-time enables more efficient and effective navigation. Finally, the system's modular design and use of affordable components make it a cost-effective solution for vacuum cleaning robots.

This project seeks to contribute to the growing field of robotics and artificial intelligence, with a focus on the development of practical and cost-effective solutions for household cleaning robots. By providing a more efficient and effective obstacle avoidance system, this project aims to enhance the performance, safety, and user experience of vacuum cleaning robots.


PROBLEM STATEMENT
Current vacuum cleaning robots employ a combination of infrared sensors and bumper sensors to detect obstacles. The infrared sensors emit infrared light and detect reflections from nearby objects, while the bumper sensors detect physical contact with obstacles. However, these sensors have limitations. Infrared sensors can be affected by environmental factors such as lighting and texture, while bumper sensors only detect obstacles after physical contact has been made.

As a result, current vacuum cleaning robots often rely on pre-programmed navigation patterns and random navigation to avoid obstacles. However, this approach can lead to inefficient cleaning paths, missed spots, and increased risk of collisions.

By addressing the limitations of current systems, this project aims to enhance the performance, safety, and user experience of vacuum cleaning robots.


OBJECTIVES OF THE STUDY
Main Objectives
The main objective of this study is to design and develop an efficient obstacle avoidance system for vacuum cleaning robots.



Specific Objectives
1. To investigate the current limitations of obstacle avoidance systems in vacuum cleaning robots.
2. To design and develop an obstacle avoidance system using ultrasonic sensors and Arduino UNO R3 microcontroller.
3. To evaluate the performance and effectiveness of the proposed system.

Research Question
What is the effectiveness of an obstacle avoidance system using ultrasonic sensors and Arduino UNO R3 microcontroller in enhancing the navigation and cleaning efficiency of vacuum cleaning robots?


SIGNIFICANCE OF THE STUDY
This study is significant because it aims to address the current limitations of obstacle avoidance systems in vacuum cleaning robots. The proposed system has the potential to enhance the navigation and cleaning efficiency of vacuum cleaning robots, making them more reliable and effective in various environments. The findings of this study can contribute to the development of more advanced and efficient cleaning robots, ultimately improving the quality of life for individuals who rely on these robots for cleaning tasks.
CONTEXT SCOPE
The study focuses on the design and development of an efficient obstacle avoidance system for vacuum cleaning robots.

Geographical Scope	
The study is limited to any standard workshop setting, with the prototype being tested in a controlled environment within Nigeria.

Time Scope
The study is theoretical and based on simulation so it is expected to be completed within 1 week, while the physical aspect should be completed in the span of 6 weeks.





# CHAPTER TWO (LITERATURE REVIEW)
INTRODUCTION

The development of efficient obstacle avoidance systems for vacuum cleaning robots has been an active area of research in recent years. With the increasing demand for autonomous cleaning solutions, researchers have explored various technologies and methods to enable robots to navigate and clean effectively in complex environments.

Existing studies have investigated the use of different sensors and algorithms for obstacle detection and avoidance. For instance, Everett and Gage used infrared sensors and artificial neural networks to enable a robot to navigate through cluttered spaces (1995).

Despite these advancements, there is still a need for more efficient and reliable obstacle avoidance systems that can adapt to changing environments. This literature review aims to provide an overview of the current state of research on obstacle avoidance systems for vacuum cleaning robots, highlighting the strengths and limitations of existing approaches and identifying areas for future research.


ULTRASONIC SENSORS
Ultrasonic sensors have emerged as a reliable and efficient solution for obstacle detection in vacuum cleaning robots. These sensors operate by emitting high-frequency sound waves and measuring the time-of-flight and intensity of the reflected signals. This information is then used to calculate the distance and orientation of obstacles in the environment.

Components
1. Trigger Component: This component sends out high-frequency ultrasonic sound waves (typically in the range of 40 kHz) into the environment.
2. Echo Component: This component receives the reflected sound waves that bounce back from obstacles in the environment.
Fig1: Ultrasonic Sensor
                               





Principle of Ultrasonic Sensor
1. The trigger component sends out a high-frequency ultrasonic sound wave.
2. The sound wave travels through the air and hits an obstacle.
3. The obstacle reflects the sound wave back to the sensor.
4. The echo component receives the reflected sound wave.
5. The sensor measures the time difference between when the trigger component sent out the sound wave and when the echo component received the reflected sound wave.
6. Using the speed of sound (approximately 343 m/s at room temperature and atmospheric pressure), the sensor calculates the distance of the obstacle from the sensor.

By measuring the time-of-flight and intensity of the reflected sound waves, ultrasonic sensors can detect obstacles and calculate their distance, orientation, and size.
Fig2: Principle of an ultrasonic sensor
Advantages
1. High accuracy: Ultrasonic sensors can detect obstacles with high accuracy, even in cluttered environments.
2. Low cost: Compared to other sensing technologies, ultrasonic sensors are relatively inexpensive.
3. Easy integration: Ultrasonic sensors are simple to integrate into robotic systems, making them a popular choice for obstacle detection.


Applications in Vacuum Cleaning Robots
1. Obstacle avoidance: Ultrasonic sensors can be used to detect and avoid obstacles, such as furniture, walls, and stairs.
2. Navigation: By detecting the distance and orientation of obstacles, ultrasonic sensors can help vacuum cleaning robots navigate through complex environments.
3. Mapping: Ultrasonic sensors can be used to create maps of the environment, allowing vacuum cleaning robots to optimize their cleaning routes.



Limitations
1. Range limitations: Ultrasonic sensors have limited range and may not detect obstacles at long distances.
2. Interference: Ultrasonic sensors can be affected by interference from other sound sources, such as background noise.

Overall, ultrasonic sensors offer a promising solution for obstacle detection in vacuum cleaning robots. Their high accuracy, low cost, and ease of integration make them an attractive choice for robotic navigation and obstacle avoidance systems.

RELATED WORK DONE
Ultrasonic sensors play a crucial role in enabling vacuum robots and other obstacle-avoiding robots to navigate safely through their environments. These sensors use high-frequency sound waves to detect and measure the distance of objects in their surroundings.
The process begins with the transmission of high-frequency sound waves by the ultrasonic sensor. When these sound waves hit an object, they bounce back and return to the sensor, which detects the reflected sound waves and measures the time difference between when the sound waves were sent and when they were received.
Using the speed of sound, the sensor calculates the distance of the object from the sensor. This information is then used by the robot to adjust its navigation accordingly, allowing it to avoid collisions and navigate safely.
In vacuum robots, ultrasonic sensors are particularly useful for detecting obstacles such as furniture, walls, and stairs. By detecting these obstacles and measuring their distance, the robot can adjust its cleaning path and avoid getting stuck or damaged.
Similarly, ultrasonic sensors are used in other obstacle-avoiding robots, such as autonomous mobile robots, drones, and self-driving cars, to detect and respond to obstacles in their / environments. Overall, ultrasonic sensors provide a reliable and efficient means of obstacle detection and avoidance, enabling robots to navigate safely and effectively.








# CHAPTER THREE
SYSTEM COMPONENTS

The ultrasonic sensors detect obstacles and measure their distance from the robot. The microcontroller processes the sensor data and controls the robot's movements. The vacuum cleaning robot platform provides the base for the robot, while the motor drivers control the speed and direction of the wheels and motors. The wheels and motors enable the robot to move around and navigate through its environment. Together, these components work in harmony to enable the robot to avoid obstacles and clean efficiently.
FIG3: SCHEMATIC OF THE SYSTEM
FIG4: COMPONENTS OF THE SYSTEM
 

ARDUINO UNO R3
The Arduino Uno R3 is a microcontroller board based on the ATmega328P, a high-performance 8-bit AVR microcontroller. It features 14 digital input/output pins, 6 analogue inputs, a 16 MHz crystal oscillator, a USB connection, and a power jack. The Arduino Uno R3 is a popular choice for DIY electronics projects, robotics, and prototyping due to its ease of use, flexibility, and affordability.
One of the key advantages of the Arduino Uno R3 is its simplicity, making it an ideal platform for beginners to learn programming and electronics. The board is also highly extensible, with a wide range of libraries and shields available for tasks such as wireless communication, motor control, and sensor integration.
The Arduino Uno R3 plays a crucial role in the development of the obstacle avoidance system for the vacuum cleaning robot, as it serves as the brain of the system. The microcontroller board is responsible for processing the data from the ultrasonic sensors, which detect obstacles and measure their distance from the robot.
In the context of the obstacle avoidance system, the Arduino Uno R3 is programmed to read data from the ultrasonic sensors, calculate the distance of obstacles, and control the motors to navigate around them. The board's flexibility and customizability make it an ideal choice for this application, as it allows for easy modification and refinement of the system.
FIG5: ARDUINO UNO R3 BOARD







LCD 16x2
The LCD16x2 is a liquid crystal display module that provides a simple and effective way to display text and numerical data. It features a 16-character by 2-line display, making it ideal for displaying short messages, sensor readings, and other data. The LCD16x2 is a popular choice for DIY electronics projects, robotics, and prototyping due to its ease of use, low cost, and compatibility with a wide range of microcontrollers.

One of the key advantages of the LCD16x2 is its simplicity, making it an ideal component for beginners to learn about display technology and user interface design. The module is also highly versatile, with a wide range of commands and functions available for customizing the display.

The LCD16x2 plays a crucial role in the development of the obstacle avoidance system for the vacuum cleaning robot, as it provides a user-friendly interface for displaying sensor data and system status. The display module is connected to the Arduino Uno R3, which sends data to the LCD16x2 for display. In the context of the obstacle avoidance system, the LCD16x2 is used to display data such as obstacle distance, sensor readings, and system status, providing the user with valuable information about the robot's operation. The module's flexibility and customizability make it an ideal choice for this application, as it allows for easy modification and refinement of the display interface.
FIG6: LCD 16x2
 

LED (YELLOW)
The LED (Yellow) is a light-emitting diode that provides a visual indication of the system's status. It features a bright yellow colour and is a popular choice for DIY electronics projects, robotics, and prototyping due to its ease of use, low cost, and compatibility with a wide range of microcontrollers.

One of the key advantages of the LED (Yellow) is its simplicity, making it an ideal component for beginners to learn about visual indicators and user interface design. The LED is also highly versatile, with a wide range of applications in electronics and robotics.

The LED (Yellow) plays a crucial role in the development of the obstacle avoidance system for the vacuum cleaning robot, as it provides a visual indication of the system's status. The LED is connected to the Arduino Uno R3, which controls the LED's state based on the system's status. In the context of the obstacle avoidance system, the LED (Yellow) is used to indicate when an obstacle is detected, providing a visual warning to the user. The LED's flexibility and customizability make it an ideal choice for this application, as it allows for easy modification and refinement of the visual indicator.
FIG7: LED (YELLOW)
 
DC MOTOR	
The DC Motor is a type of electric motor that converts direct current (DC) electrical energy into mechanical energy. It is a popular choice for DIY electronics projects, robotics, and prototyping due to its ease of use, low cost, and compatibility with a wide range of microcontrollers.

One of the key advantages of the DC Motor is its simplicity, making it an ideal component for beginners to learn about motor control and robotics. The DC Motor is also highly versatile, with a wide range of applications in electronics and robotics, including robotic arms, vehicles, and conveyor systems.

The DC Motor plays a crucial role in the development of the obstacle avoidance system for the vacuum cleaning robot, as it provides the mechanical energy needed to propel the robot forward. The DC Motor is connected to the Arduino Uno R3, which controls the motor's speed and direction based on the sensor data. In the context of the obstacle avoidance system, the DC Motor is used to drive the robot's wheels, allowing it to navigate around obstacles and avoid collisions. The motor's flexibility and customizability make it an ideal choice for this application, as it allows for easy modification and refinement of the robot's movement.
FIG8: DC MOTOR
 
H-BRIDGE MOTOR DRIVER
The H Bridge Motor Driver is a type of electronic circuit that enables the control of DC motors in both forward and reverse directions. It is a popular choice for DIY electronics projects, robotics, and prototyping due to its ease of use, low cost, and compatibility with a wide range of microcontrollers.
One of the key advantages of the H Bridge Motor Driver is its ability to control the speed and direction of DC motors, making it an ideal component for applications that require precise motor control. The H Bridge Motor Driver is also highly versatile, with a wide range of applications in electronics and robotics, including robotic arms, vehicles, and conveyor systems.

The H Bridge Motor Driver plays a crucial role in the development of the obstacle avoidance system for the vacuum cleaning robot, as it enables the control of the DC motors that propel the robot forward. The H Bridge Motor Driver is connected to the Arduino Uno R3, which sends signals to the driver to control the motor's speed and direction. In the context of the obstacle avoidance system, the H Bridge Motor Driver is used to drive the robot's wheels, allowing it to navigate around obstacles and avoid collisions. The driver's flexibility and customizability make it an ideal choice for this application, as it allows for easy modification and refinement of the robot's movement.
FIG9: H-BRIDGE MOTOR DRIVER
 
ULTRASONIC SENSOR
The Ultrasonic Sensor is a type of non-contact proximity sensor that uses high-frequency sound waves to detect and measure the distance of objects. It is a popular choice for DIY electronics projects, robotics, and prototyping due to its ease of use, low cost, and compatibility with a wide range of microcontrollers.

One of the key advantages of the Ultrasonic Sensor is its ability to provide accurate and reliable distance measurements, making it an ideal component for applications that require obstacle detection and avoidance. The Ultrasonic Sensor is also highly versatile, with a wide range of applications in electronics and robotics, including robotic navigation, obstacle avoidance, and proximity detection.

The Ultrasonic Sensor plays a crucial role in the development of the obstacle avoidance system for the vacuum cleaning robot, as it provides the primary means of detecting and measuring the distance of obstacles. The Ultrasonic Sensor is connected to the Arduino Uno R3, which processes the sensor data and controls the robot's movements accordingly. In the context of the obstacle avoidance system, the Ultrasonic Sensor is used to detect obstacles and measure their distance from the robot, allowing the robot to navigate around them and avoid collisions. The sensor's flexibility and customizability make it an ideal choice for this application, as it allows for easy modification and refinement of the obstacle detection and avoidance algorithm.
FIG10: ULTRASONIC SENSOR
 
RESISTOR
The Resistor is a fundamental electronic component that opposes the flow of electric current. It is a crucial component in a wide range of electronic circuits, including voltage dividers, filters, and amplifiers. The Resistor is available in various resistance values, ranging from a few ohms to several megohms, making it a versatile component for various applications.
One of the key advantages of the Resistor is its ability to regulate voltage and current levels in electronic circuits. By carefully selecting the resistance value, designers can create circuits that operate within specific voltage and current ranges. The Resistor is also a low-cost component, making it an ideal choice for prototyping and production.
In the context of the obstacle avoidance system for the vacuum cleaning robot, Resistors play a crucial role in voltage division, signal attenuation, and current limiting. They are used to divide the voltage levels from sensors, attenuate signal amplitudes, and limit current flows to prevent damage to sensitive components. The Resistor's flexibility and availability in various resistance values make it an essential component for electronic circuit design and development.
FIG11: RESISTOR
 
DESIGN OF SYSTEM
This schematic represents a well-integrated system using an Arduino Uno microcontroller. The design focuses on combining sensor input, actuation, and output display, making it suitable for automation projects such as obstacle-avoidance robots, distance-based motor control systems, or smart vehicles. Below is a detailed description of the system design and its functionalities.
System Functionality
1.	Sensor-Driven Control:
o	The ultrasonic sensor continuously measures distances to objects and sends data to the Arduino.
o	The Arduino processes the data to decide whether to stop the motors, change their direction, or adjust their speed.
2.	Motor Actuation:
o	The motor driver uses the Arduino's control signals to regulate the motors.
o	It allows for forward, backward, and turning movements, enabling the system to navigate or respond to obstacles dynamically.


3.	Visual Feedback:
o	The LCD displays key information such as system status, distance to obstacles, or operational mode.
o	This makes the system more user-friendly and provides valuable debugging information during development.
4.	Interactive Adjustments:
o	The potentiometer allows the user to fine-tune the LCD contrast, improving the user interface's readability.
o	It adds a manual control layer to the otherwise automated system.
5.	Indicator Feedback:
o	The LED acts as an operational indicator, providing immediate visual cues about the system's state. For instance: 
	A steady light may indicate normal operation.
	Blinking could signal a detected obstacle or an error.


Functionality of the Design
1.	Scalability: Additional sensors or modules can be integrated with the Arduino, enhancing the system's functionality.
2.	Real-Time Feedback: The LCD provides real-time data, improving usability and debugging capabilities.
3.	Interactivity: The potentiometer and LED make the system more intuitive for users.
4.	Precision: The motor driver and ultrasonic sensor enable precise and adaptive control over movement.
FIG12: PROTEUS SIMULATION OF THE SYSTEM

WORKING OF THE SYSTEM
When powered on, the Arduino Uno initializes all connected components, and the LCD displays a message on system status to indicate that the system is ready for operation. The LED will turn on to indicate functionality of the system.
The ultrasonic sensor emits sound waves and measures the time taken for the echo to return after hitting an object, sending this distance data to the Arduino via its trigger and echo pins. The Arduino processes the signal to calculate the distance to the object using a predefined formula.
The Arduino compares the measured distance against predefined thresholds programmed in the firmware. If the distance is safe, the motors are allowed to run. However, if an obstacle is detected, the Arduino sends a command to the motor driver to perform a turning functionality.
Based on the distance data, the motor driver receives control signals from the Arduino to regulate the motors' speed and direction. The LCD display continuously updates with real-time data, such as the measured distance, motor status, or system messages. The LED indicator provides visual feedback depending on the system's state.
The system continuously monitors its surroundings using the ultrasonic sensor and dynamically controls the motors to avoid obstacles. The LCD and LED provide valuable feedback to the user, while the potentiometer improves usability. This makes the design an ideal candidate for obstacle-avoiding robots, smart vehicles, or automated distance-controlled systems.
In operation, the system powers on, and the LCD displays if an obstacle is detected or not. The ultrasonic sensor detects an object within a certain range, and the Arduino calculates the distance and determines whether it is within the critical range. If so, the Arduino sends a signal to the motor driver to alternate the motors and perform a turning sequence and continuously blinks the LED to indicate an obstacle. Once the obstacle is removed, the system resumes normal operation, and the motors move forward and the LED stops blinking and stays on.
FIG13: LCD RUNNING SIMULATION






# CHAPTER FOUR
SYSTEM CODE
```
#include <LiquidCrystal.h>
int trig = 1;
int echo = 0;
int ma1 = 7;
int ma2 = 6;
int mb1 = 3;
int mb2 = 2;
int led = 4;
const int rs = 13, en = 12, d4 = 11, d5 = 10, d6 = 9, d7 = 8;
LiquidCrystal lcd(rs, en, d4, d5, d6, d7);

void Right() {
  lcd.setCursor(0, 1);
  lcd.print("OBSTACLE FOUND");
  delay(300);
  lcd.setCursor(0, 1);
  lcd.print("TURNING........");
  digitalWrite(ma1, HIGH);
  digitalWrite(ma2, LOW); 
  digitalWrite(mb1, LOW);
  digitalWrite(mb2, HIGH); 
  analogWrite(5, 225);
}

void Forward() {
  lcd.setCursor(0, 1);
  lcd.print("MOVING FOWARD");
  digitalWrite(ma1, HIGH);
  digitalWrite(ma2, LOW); 
  digitalWrite(mb1, HIGH);
  digitalWrite(mb2, LOW); 
  analogWrite(5, 225);
}

void setup() {
  pinMode(echo, INPUT);
  pinMode(trig, OUTPUT);
  pinMode(ma1, OUTPUT);
  pinMode(ma2, OUTPUT);
  pinMode(mb1, OUTPUT);
  pinMode(mb2, OUTPUT);
  pinMode(led, OUTPUT);
}

void loop() {
  digitalWrite(trig, LOW);
  delay(3);
  digitalWrite(trig, HIGH);
  delay(10);
  digitalWrite(trig, LOW);
  
  int duration = pulseIn(echo, HIGH);
  int distance = duration * 0.034/2;
    lcd.begin(16, 2);
  
  lcd.print("Distance: ");
  lcd.print(distance);

  if (distance >= 500) {
    Forward();
    digitalWrite(led, HIGH);
  }

  else {
    Right();
    digitalWrite(led, LOW);
    delay(150);
    digitalWrite(led, HIGH);
    delay(150);
  }
}
```
FIG14: PREVIEW OF THE CODE

# Function of the code
This code uses an ultrasonic sensor to detect obstacles and avoid them. The Trigger pin sends out a sound wave and the echo pin receive the echo of that sound; it then calculates the amount of time it took and use that to get the distance. When the distance is between the robot and the obstacle is high, it runs the “Forward()” function which was coded to make both motors rotate clock wise, but when the distance is low, the code runs the “Right()” function which was coded to make one motor rotate clock wise and the other one rotate anti clockwise cause the robot to move left or right, and avoid the obstacle.
RESULT OF THE SYSTEM
The result of the system is an intelligent obstacle avoidance robot that can navigate through its environment while avoiding collisions with obstacles. The robot uses an ultrasonic sensor to detect obstacles and measure their distance, and an Arduino microcontroller to process the sensor data and control the robot's movements.
- The robot can detect obstacles and avoid collisions.
- The robot can move forward and turn right based on the distance of the obstacles.
- The robot provides visual feedback through an LCD display, showing the distance of the obstacles and the robot's status.
- The robot provides visual indication through an LED, indicating when an obstacle is detected and when the robot is turning.
- The system demonstrates a simple and effective solution for obstacle avoidance in robotics.

Overall, the system demonstrates a successful implementation of an obstacle avoidance robot using Arduino and ultrasonic sensors.

# CHAPTER FIVE

CONCLUSION
An obstacle avoidance robot is a type of robot that is designed to navigate through a cluttered environment without colliding with obstacles. These robots use sensors and algorithms to detect and avoid obstacles in their path.

An obstacle avoidance robot operates by using sensors to detect obstacles in its environment. The sensors send data to a microcontroller or computer, which uses algorithms to interpret the data and determine the best course of action to avoid the obstacle. The robot then uses its motors and actuators to execute the avoidance manoeuvre.

The robot uses an ultrasonic sensor to detect obstacles in its environment. The sensor sends a high-frequency sound wave and listens for the echo. The time it takes for the echo to return is proportional to the distance to the obstacle.

The robot uses a microcontroller to interpret the data from the ultrasonic sensor and determine the best course of action to avoid the obstacle. The microcontroller sends signals to the motor to turn it off and then on to avoid the obstacle.

The robot uses a DC motor to move forward and avoid obstacles. The motor is controlled by the microcontroller, which sends signals to turn the motor off and on.

# RECOMMENDATION
To enhance the obstacle avoidance robot, add an infrared sensor to complement the existing ultrasonic sensor. This multi-sensor approach will improve accuracy and reliability in detecting obstacles. Modify the code to integrate infrared data and adjust the obstacle detection algorithm accordingly, enabling the robot to navigate more effectively.


# REFERENCES	
1. Borenstein, J. (1991). The Navlab: A Testbed for Research in Autonomous Navigation. Kluwer Academic Publishers.
2. Brooks, R. A. (1986). A Robust Layered Control System for a Mobile Robot. IEEE Journal of Robotics and Automation, 2(1), 14-23.
3. Dudek, G., & Jenkin, M. (2010). Computational Principles of Mobile Robotics. Cambridge University Press.
4. Everett, H. R. (1995). Sensors for Mobile Robots: Theory and Application. A K Peters.
5. Fu, K. S., Gonzalez, R. C., & Lee, C. S. G. (1987). Robotics: Control, Sensing, Vision, and Intelligence. McGraw-Hill.
6. Hebert, M. (2000). Active and Passive Range Sensing for Robotics. Springer.
7. Khatib, O. (1986). Real-Time Obstacle Avoidance for Manipulators and Mobile Robots. International Journal of Robotics Research, 5(1), 90-98.
8. Latombe, J. C. (1991). Robot Motion Planning. Kluwer Academic Publishers.
9. Lozano-Pérez, T. (1983). Spatial Planning: A Configuration Space Approach. IEEE Transactions on Computers, 32(3), 108-120.
