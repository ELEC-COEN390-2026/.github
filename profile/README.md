# ELEC/COEN390 - Team 13 - Winter 2026
# SeatFinder

## Team Members
* **Ethan Rahal:** 40316235
* **Sbaz Ali Khan:** 40272349
* **Kareem Dadouche:** 40226983
* **Amine Mefti:** 40281614
* **Yansong Li:** 40212154

## About the Project
We are building a live occupancy tracking system so students don't have to walk all the way across campus just to find out a study area is completely full. 

To ensure high reliability and prove our core detection logic, we have intentionally scoped our initial prototype to a 3-seat micro-zone. We are using an LD2450 mmWave radar to track sustained micro-motions. This means the system actually knows if someone is sitting at a desk studying, rather than just logging a false positive when someone walks past. 

The sensor feeds this data to an ESP32, which pushes state changes to the cloud, and our mobile app updates the available seat count in real time. Because our architecture relies on a modular cloud database, scaling this project up to cover an entire library floor in the future is incredibly straightforward: it simply requires deploying more sensor nodes without needing to overhaul the app or backend.

## Technologies
* **Hardware:** ESP32 Microcontroller, HLK-LD2450 mmWave Radar Sensor, and a custom 3D-printed mount.
* **Backend / Cloud:** Firebase Realtime Database and C++ for the ESP32 firmware.
* **Frontend:** Android Studio (Java) for the app.
* **Simulation:** Python
