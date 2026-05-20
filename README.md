#  Sam's Smart Automobile Maze Solver

A robotics project built at Al-Ahliyya Amman University for the Robotics Programming course under Prof. Ayman Elshenawy.

##  Introduction
A small robot that autonomously solves a maze by detecting walls using sensors and choosing the correct path using a decision-making algorithm.

##  Goals
- Autonomously solve the maze
- Avoid wall collisions
- Make decisions at maze intersections
- Enhance programming and engineering skills
- Apply basic artificial intelligence concepts

##  Hardware Components
- Arduino A3
- Ultrasonic Sensor (HC-SR04)
- 2 DC Motors
- H-Bridge Motor Driver (L298N)
- Lithium Battery
- Chassis (Robot Base)

##  Code Logic
- If no obstacle → Move forward
- If obstacle detected:
  - Stop and back up
  - Scan left → if clear, go left
  - Scan right → if clear, go right
  - If both blocked → turn around

##  Hardware Integration
- Ultrasonic sensor detects distance in cm
- L298N driver manages motor speed and direction
- Arduino A3 processes input and controls logic

##  Pin Connections
| Component | Pin |
|---|---|
| Ultrasonic Trig | Pin 9 |
| Ultrasonic Echo | Pin 8 |
| Motor Left A | Pin 6 |
| Motor Left B | Pin 11 |
| Motor Right A | Pin 3 |
| Motor Right B | Pin 5 |

##  What Worked Well
- Robot successfully avoided obstacles and made decisions
- Ultrasonic sensor readings were reliable for most distances

##  Challenges
- Right motor was not working properly
- Finding the right key logic and tuning

##  Future Work
- Add extra sensors for better navigation accuracy
- Integrate Bluetooth or Wi-Fi for remote control
- Add a camera for image recognition
- Apply smarter algorithms like left-hand or right-hand rule
