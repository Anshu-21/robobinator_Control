<h1>♻️ Smart Waste Segregation System with Robotic Arm </h1><br>
<h3>📌 Project Overview</h3>
This project is developed for Smart India Hackathon (SIH). It is a Waste Segregation System that uses a robotic arm to automatically detect, classify, and segregate waste into different categories.

Base with 3 compartments → Biodegradable, Recyclable, and Non-recyclable.

Robotic Arm (SolidWorks + ROS/Gazebo) → Picks and places the detected waste.

Sensors → Ultrasonic sensor detects waste nearby, Camera captures the object.

Machine Learning Model → Classifies waste category from the camera feed.

Control System → Arduino/Raspberry Pi controls motors and sensors.

🛠️ Features

✅ Automated waste detection using ultrasonic sensor

✅ Waste classification using ML model (biodegradable, recyclable, non-recyclable)

✅ Robotic arm simulation in ROS + Gazebo

✅ Circuit design & control code in Tinkercad + Arduino

✅ 3D design of base and robotic arm in SolidWorks

📂 Repository Structure

```
Waste-Segregation-Robot/
│── README.md                 # Project documentation
│── /circuit/                 # Tinkercad circuit diagram + Arduino code
│   ├── circuit_diagram.png
│   ├── control_code.ino
│
│── /simulation/              # ROS + Gazebo files
│   ├── arm_urdf.launch
│   ├── world/
│   ├── config/
│
│── /ml_model/                # ML model for waste classification
│   ├── dataset_link.txt
│   ├── waste_classifier.ipynb
│
│── /design/                  # SolidWorks design files
│   ├── base_with_compartments.sldprt
│   ├── robotic_arm.sldasm
│
│── /docs/                    # Extra project docs (report, PPTs, etc.)
```





⚡ Circuit Design (Tinkercad)

Ultrasonic Sensor → Detects object distance

Small Servo Motors → Control robotic arm joints & gripper

High Torque Servo Motors → For base 

Arduino UNO → Controls sensors and actuators

Motor Driver → Drives arm motors

<img width="998" height="667" alt="{0FD476C2-5709-4A2B-8B15-53B0001A0293}" src="https://github.com/user-attachments/assets/0da46db5-a9fc-4d77-a294-4abf6e693002" />





🤖 Simulation (ROS + Gazebo)

Robotic arm designed and simulated in ROS Noetic + Gazebo

URDF model created for robotic arm and environment

Launch file: arm_urdf.launch

The simulation shows the robotic arm detecting waste and placing it in the right compartment


🚀 How to Run</br>
1️⃣ Arduino Code (Tinkercad or Hardware)

-> Upload control_code.ino to Arduino UNO

-> Connect sensors and motors as per circuit_diagram.png

-> Run simulation in Tinkercad OR test on real hardware

2️⃣ ROS + Gazebo Simulation

-> cd ~/catkin_ws/src

-> catkin_make

-> roslaunch Robobinator arm_urdf.launch

📊 Workflow

-> Ultrasonic sensor detects waste

-> Camera captures image of waste

-> ML model classifies waste type

-> Robotic arm picks and places object in the correct compartment

-> Compartments collect segregated waste

Circuit Diagram

.<img width="963" height="725" alt="{A95840E2-A666-4E8B-B8B1-A64865A1C6C9}" src="https://github.com/user-attachments/assets/f2297e84-358a-4174-b3d5-c5cc4d2187ab" />

👨‍💻 Team

Anshu Kumar – Control System and Simulation (TinkerCad, ROS)
