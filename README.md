# UR3e Robot Python Connection Code
This repository contains the Python code for establishing a connection between the UR3e robot and our gesture recognition system. The provided code demonstrates the preliminary structure of the hardware connection and the communication protocols between the robot and the control system.

Overview
The connection between the UR3e robot and the gesture recognition system is established using Python. We connect the UR arm via a network connection using the robot’s IP address and designated control port.

For the Universal Robot (UR3e), the primary communication is handled through TCP/IP sockets, which allow us to send control commands and receive status updates from the robot. Using Python's socket library, we can open a communication channel between the robot's IP address and other predefined ports.

Once the connection is established, the script sends movement commands to the robot, such as Cartesian pose alterations. This enables users to manipulate the robot's position and orientation through socket communication.

In addition, Modbus TCP is used to retrieve key status data, including joint angles and tool center point (TCP) positions, allowing us to monitor and adjust the robot's behavior based on real-time feedback.

Features
Establishes a network connection between the UR3e robot and the control system using Python.
Controls the robot's movement through Cartesian pose alterations.
Modbus TCP retrieves and monitors joint angles and TCP positions.
Communicates with the gripper for controlling grip speed, force, and position.
Setup
Clone this repository to your local machine:

bash
คัดลอกโค้ด
git clone https://github.com/bunchart1368/final-project
Install necessary Python libraries:

bash
คัดลอกโค้ด
pip install pymodbus
Run the provided Python scripts to establish the robot and gripper connections.

Code and Simulation Files
You can access the full code for robot and gripper connection, along with simulation files, through this GitHub repository.

