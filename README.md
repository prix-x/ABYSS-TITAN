#Abyss Titan

A 4kg heavy-duty Tug-of-War robot built for high traction and strength. It uses high-torque Johnson motors and heavy wiring to handle the high current demands.

## Hardware 

This bot is built tough to handle heavy pulls without breaking or burning out:

* **Motors:** High-torque Johnson Geared Motors.
* **Power Control:** Heavy-duty BTS7960 43A Dual H-Bridge motor drivers to handle high stall currents.
* **Wiring Rail:** Thick 14 AWG wires utilized across the high-current loops to prevent voltage drops.
* **Chassis Layout:** Metal chassis with screws to secure everything, with weights that add up to the 4KG Limit.

---

## 💻 Firmware & Control Features

The onboard **ESP32** is programmed using Arduino IDE to allow wireless mobile control and smooth power delivery:

* **Wireless Interface:** Configured via `BluetoothSerial.h` to pair directly with a smartphone under the local broadcast name `"Abyss Titan"`.
* **Hardware PWM Driving:** Operates at `5000Hz` using the ESP32's native `ledcSetup` and `ledcAttachPin` commands, ensuring completely smooth throttle response and removing high-pitched motor hum.

---

## 🗺️ Project Roadmap

- [x] Assemble physical chassis and balance center of mass
- [x] Wire high-current electronics layout (Johnson Motors + BTS7960)
- [x] Complete core ESP32 control firmware with Bluetooth handling
- [x] Record design and operation timelapse
- [ ] Implement wireless control application layout
- [ ] Run full-load field traction tests
