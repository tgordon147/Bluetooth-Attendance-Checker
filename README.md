***Bluetooth Attendance Checker (Mobile App)***

This repository contains the mobile application component of the Bluetooth Attendance Checker system, designed to automate and secure university attendance tracking using Bluetooth Low Energy (BLE).

***Overview***

The Bluetooth Attendance Checker mobile app allows students to authenticate and broadcast their presence in lecture halls via BLE advertisements, ensuring they are physically present to be marked as attending. The app works in conjunction with the Bluetooth Attendance Server, which verifies attendance and updates university records.

***Features***

Seamless Attendance Verification: Students simply open the app and start advertising their presence—no need for manual check-ins.
Prevention of Fraudulent Attendance: BLE technology ensures students must be physically near the lecture hall’s Attendance Server (Raspberry Pi) to register.
Low Power Consumption: Uses Bluetooth Low Energy (BLE) to minimize battery usage.
AWS & Blackboard Integration:
The app communicates with the server, which uploads attendance data to AWS-hosted Blackboard instances.
Attendance records can be automatically updated on Blackboard’s Attendance API (where available).

***How It Works***

Student Login: The app authenticates users and registers them for attendance tracking.
BLE Broadcasting: The app advertises a unique student ID via BLE, which is detected by the Raspberry Pi-based server.
Attendance Tracking: The server records the student’s presence and updates the university’s attendance system (Blackboard).

***Integration with Server***

The app is designed to work alongside the Bluetooth Attendance Server, which scans for BLE signals and uploads attendance data to AWS & Blackboard.

Related Repository
👉 Server Component: Bluetooth Attendance Server
