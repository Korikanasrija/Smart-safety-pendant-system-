# Smart-safety-pendant-system-

## 1. Project Title
**Smart Safety Pendant System using SIM800L GSM Module and NEO-6M GPS Module**

---

## 2. Project Overview
The **Smart Safety Pendant System** is a portable emergency safety device designed to help users quickly send alerts during dangerous or emergency situations. The system uses a **SIM800L GSM module** for phone calling and SMS communication, and a **NEO-6M GPS module** for obtaining real-time location coordinates.

The device is designed like a **safety pendant / wearable emergency gadget** and contains **two push buttons**:

- **Push Button 1 – Emergency Call Button**
  - Used to make a phone call to a predefined emergency contact.

- **Push Button 2 – Location Alert Button**
  - Used to fetch the current GPS location and send an alert SMS with the location to a predefined contact.

The project is especially useful for **women safety, elderly care, child safety, solo travelers, and emergency response systems**. The main idea is to provide a **quick-response emergency system** that works even when the user cannot unlock or operate a smartphone.

---

# 3. Project Description
The **Smart Safety Pendant System** is an embedded personal safety device that combines **GSM communication** and **GPS location tracking** into one compact system. It is built around a microcontroller and connected to a **SIM800L GSM module** and **NEO-6M GPS module**.

In emergency situations, the user can press one of the two buttons:

- The **Call Button** initiates an emergency phone call to a stored contact number.
- The **Location Alert Button** obtains the current GPS coordinates and sends an **SOS SMS** with a location link.

This system can be worn as a pendant or carried as a small portable unit. It offers a simple, low-cost, and practical safety solution for real-world use.

---
# DEMONSTRATION
<a href="https://go.screenpal.com/watch/cO132fnusA8">➡️For message</a>
<a href="https://go.screenpal.com/watch/cO1326nusB7">➡️For calls</a>

# 4. Objectives

## Main Objective
To design and develop a **smart safety pendant system** capable of making an emergency call and sending the user’s live location through GSM and GPS technology.

## Specific Objectives
- To develop a **portable emergency safety device** using **SIM800L** and **NEO-6M** modules.
- To implement an **emergency call feature** using a dedicated push button.
- To implement a **GPS-based location tracking and alert message feature** using a second push button.
- To send **SOS SMS alerts** containing the user’s real-time location.
- To provide a **simple and fast emergency response system**.
- To create a **low-cost safety device** for personal protection applications.

---

# 5. Problem Statement
In emergency situations such as harassment, accidents, health issues, or unsafe travel conditions, a person may not have enough time to unlock a mobile phone, open apps, and send messages manually. There is a need for a **simple one-touch emergency device** that can instantly contact trusted people and share the user’s location. This project addresses that need by creating a **smart safety pendant** with emergency call and location alert features.

---

# 6. Features
- Emergency phone call using GSM
- SMS alert with live GPS location
- Two-button emergency control
- Real-time location tracking using GPS
- Portable pendant-style safety system
- Low-cost implementation
- Easy to use during panic situations
- Can be extended to wearable and IoT safety applications

---

# 7. Components Required

## Hardware Components
- **Microcontroller board** (Arduino Uno / Nano / ESP32)
- **SIM800L GSM Module**
- **NEO-6M GPS Module**
- **2 Push Buttons**
  - Button 1: Emergency Call
  - Button 2: Location Alert / Tracking
- **2 Breadboards**
- Jumper wires
- SIM card with active GSM network
- Power supply / battery
- Resistors (optional for pull-down / pull-up button setup)
- LED / buzzer (optional for indication)

## Software Requirements
- Arduino IDE
- Embedded C / Arduino programming
- TinyGPS++ library (for GPS parsing, optional but recommended)
- SoftwareSerial library (if using Arduino Uno/Nano)

---

# 8. Technologies Used
- **Embedded Systems**
- **GSM Communication**
- **GPS Tracking**
- **Arduino Programming**
- **IoT-based Safety Concept**

---

# 9. Hardware Module Description

## 9.1 SIM800L GSM Module
The **SIM800L** is a compact GSM/GPRS module that enables:
- Sending SMS
- Making phone calls
- Receiving network information
- Communicating with the microcontroller using **AT commands**

### Role in this project
- Places an emergency call to a stored phone number
- Sends SOS alert SMS to emergency contacts

---

## 9.2 NEO-6M GPS Module
The **NEO-6M GPS module** is used to obtain the geographic coordinates of the user in real time.

### GPS data includes:
- Latitude
- Longitude
- UTC time (optional)

### Role in this project
- Provides the user’s current location
- Helps create a Google Maps location link for emergency SMS alerts

---

## 9.3 Push Buttons
Two push buttons are used as user input controls:

### Button 1 – Emergency Call Button
When pressed, it triggers the GSM module to make an emergency call.

### Button 2 – Location Alert Button
When pressed, it triggers the GPS module to fetch location data and the GSM module to send an alert SMS.

---

# 10. Working Principle
The Smart Safety Pendant System works by continuously monitoring the state of two push buttons connected to the microcontroller.

## Case 1: Emergency Call Button Pressed
1. User presses the **Emergency Call Button**.
2. Microcontroller detects the button press.
3. It sends AT commands to the **SIM800L GSM module**.
4. SIM800L dials the predefined emergency contact number.
5. The user is connected to the emergency contact.

## Case 2: Location Alert Button Pressed
1. User presses the **Location Alert Button**.
2. Microcontroller reads GPS data from the **NEO-6M module**.
3. It extracts the latitude and longitude values.
4. A message is created with the location coordinates and Google Maps link.
5. The **SIM800L module** sends the alert SMS to a predefined emergency number.

---

# 11. System Architecture

## Input Section
- Emergency Call Push Button
- Location Alert Push Button

## Processing Section
- Microcontroller (Arduino / other board)

## Communication Section
- SIM800L GSM module

## Location Section
- NEO-6M GPS module

## Output Section
- Emergency phone call
- SMS alert with GPS location

---
# 12. Advantages
-Very easy to use
-Provides immediate emergency communication
-Sends real-time location
-Useful in panic situations
-Low-cost and compact design
-Can be converted into a wearable smart pendant
-Does not depend on smartphone apps during emergency action

# 13.Limitations
-Requires GSM network availability
-GPS signal may be weak indoors
-SIM800L needs stable power due to high current bursts
-SMS delivery depends on mobile network conditions
-GPS location may take some time to lock during startup

# 14.Future Scope / Enhancements

This project can be improved further by adding:

-Buzzer alarm system
-LED indication for call/SMS status
-Rechargeable Li-ion battery
-Charging module (TP4056)
-OLED display for GPS status
-Multiple emergency contacts
-Mobile app integration
-Cloud tracking / IoT dashboard
-Voice recording
-Fall detection sensor
-Heartbeat / health sensor integration
-Hidden silent emergency mode
 
# 15.Conclusion

The Smart Safety Pendant System using SIM800L GSM and NEO-6M GPS is a practical and effective embedded safety solution for emergency situations. It combines one-touch emergency calling and real-time location alerting in a compact design. The project is highly useful in personal safety applications such as women safety, elderly assistance, and child monitoring. By using simple hardware components and GSM/GPS technology, the system provides a low-cost and reliable emergency response mechanism.
