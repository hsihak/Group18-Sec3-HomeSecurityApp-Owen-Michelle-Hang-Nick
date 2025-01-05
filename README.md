# 🏠 Home Security System Manager

## 🌟 Overview

The **Home Security System Manager** is a mobile application developed in Java for Android, enhanced with Arduino-based hardware simulations. This project provides a centralized platform for users to manage and set up home security systems, offering both software and hardware integration for a complete smart home experience. By adhering to the Command Design Pattern and SOLID principles, the app ensures modularity, scalability, and ease of use.

## ✨ Features

### Supported Security Systems
- 🔒 **Door Locks**: Lock, unlock, and set PINs remotely.
- 💡 **Lights**: Control lights with on/off functionality and timers for security simulation.
- 📹 **Cameras**: Monitor live feeds remotely.
- 🚨 **Alarms**: Activate/deactivate and adjust volume remotely.
- 🔊 **Speakers**: Communicate with visitors at the door.
- 🕵️ **Motion Detectors**: Receive real-time notifications for detected motion.

### Key Functionalities
- Centralized control for multiple security systems.
- Remote setup and management through an intuitive GUI.
- Notifications and alerts for enhanced security.
- Arduino integration for hardware simulation of app-controlled devices.

## 🤖 Arduino Integration

The app is paired with Arduino hardware to simulate real-world interactions. It controls:
- 🔒 Door lock mechanisms using servos.
- 💡 Light systems using LEDs.
- 🕵️ Motion detection using PIR sensors.
- 🚨 Alarm systems using buzzers.

Arduino connects with Firebase to synchronize app commands and hardware responses in real time.

### 🛠️ How It Works
1. The app sends user commands to Firebase.
2. The Arduino reads commands from Firebase and performs the requested action.
3. Actions include turning on/off devices, setting timers, or sending motion alerts.

## 📸 Screenshots
_Add screenshots showcasing:_
1. Dashboard displaying all connected systems.
2. Individual system management (e.g., door locks, lights).
3. Notifications and alerts for motion detection.
4. Arduino setup and interactions with app controls.

## 🖌️ Wireframes
View the application's wireframe design on Figma:  
[🎨 Security System Wireframes](https://www.figma.com/file/Piy1bUa3Vj8Mz7u4ZUiv9H/Security-System-Wireframes?type=design&node-id=0%3A1&mode=design&t=XF4SqTj5mMpTfXRj-1)

## 🎥 Demo Video
Watch the application and Arduino simulation demo on YouTube:  
[![SafeUp App Demo](https://markdown-videos-api.jorgenkh.no/url?url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DuZ00hN2tV-s)](https://www.youtube.com/watch?v=uZ00hN2tV-s)

## 🚀 Getting Started

### Prerequisites
- 🖥️ Java Development Kit (JDK) 11 or later.
- 🛠️ Android Studio.
- ⚙️ Gradle build system.
- 🤖 Arduino IDE.
- 🔌 Required hardware: Arduino Uno/Nano, PIR sensor, LEDs, servos, and buzzer.

### Installation

#### Software
1. Clone this repository:
   ```bash
   git clone https://github.com/hsihak/Group18-Sec3-HomeSecurityApp-Owen-Michelle-Hang-Nick.git
2. Open the project in Android Studio.
3. Sync the Gradle build files.
4. Build and run the application on an emulator or physical device.

### Arduino

1. Navigate to the Arduino_Code folder.
2. Open the .ino file in the Arduino IDE.
3. Connect your Arduino device and upload the code.
4. Ensure Firebase credentials are configured in the Arduino code for synchronization.

### 🛠️ Design: Class Diagram

Here is the class diagram illustrating the structure and relationships within the application:

1. **Command Design Pattern**:
   - `Command` Interface: Defines the methods `executeOn()`, `executeOff()`, and `executeSetup()`.
   - Concrete Command Classes:
     - `DoorLockCommand`
     - `LightCommand`
     - `CameraCommand`
     - `AlarmCommand`
     - `SpeakerCommand`
     - `MotionDetectorCommand`
   - Receiver Classes:
     - `DoorLock`
     - `Light`
     - `Camera`
     - `Alarm`
     - `Speaker`
     - `MotionDetector`
   - `Remote` Class: Invokes methods from the command objects.

  ![image](https://github.com/user-attachments/assets/26affd4c-139e-47c2-869b-50cff5c8afc1)



### 🏆 Acknowledgments
Special thanks to:

Our team members for their hard work and dedication.
Professors and mentors for guidance throughout the project.
   
