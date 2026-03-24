# Ball-on-Plate System (3RRS Manipulator)

## 📌 Overview
This project presents a control system for a ball-on-plate setup using a 3RRS parallel manipulator, PID controller and an Arduino UNO microcontroller.  
The objective was to stabilize the ball at a desired position and to track simple motion trajectories.

<img width="300" src="https://github.com/user-attachments/assets/5a16e375-8e2b-4d3b-a7fc-4d6dcec1f0aa" />

---

## 🎯 Objectives
- Stabilization of the ball at position (0,0)
- Implementation of PID control in two axes
- Trajectory tracking (circle, square)
- Implementation on a real physical system

---

## 🛠️ Tools & Technologies
- MATLAB / Simulink
- Arduino IDE (C++)
- Signal filtering (FIR)

---

## 🧠 My Contributions
- Developed a mathematical model of the system
- Tuned PID controller parameters
- Implemented stepper motor control
- Developed a ball position detection algorithm
- Designed an FIR filter for signal processing
- Analyzed the potential application of ADRC control

---

## 📊 Results

### Step Response
- Settling time: ~2 s for a 25 mm step
- Test case: transition from (25,25) → (0,0)

<img width="400" src="https://github.com/user-attachments/assets/6be00de1-8fcb-4ea3-a438-ef2cae340720" />

---

### Disturbance Rejection
- The system stabilizes the ball after external disturbance (manual push)

<img width="400" src="https://github.com/user-attachments/assets/662a6bfb-986c-46cd-9281-b41ddc3d0b15" />

---

### Trajectory Tracking
- Successful tracking of circular and square trajectories
- Limited accuracy observed

<img width="300" src="https://github.com/user-attachments/assets/6d6e8734-25c3-461f-b381-3cc0a7beb066" />

---

## 🎥 Video Demonstration
The system stabilizes the ball, compensates disturbances and follows predefined trajectories.

### Disturbance Rejection
[![Demo](https://img.youtube.com/vi/wO5LeluoGk4/0.jpg)](https://www.youtube.com/watch?v=wO5LeluoGk4)

### Square Trajectory
[![Trajectory](https://img.youtube.com/vi/QgTJa6kDOz0/0.jpg)](https://www.youtube.com/watch?v=QgTJa6kDOz0)

### Circular Trajectory
[![Disturbance](https://img.youtube.com/vi/Sv3K1zqYGdE/0.jpg)](https://www.youtube.com/watch?v=Sv3K1zqYGdE)

---

## 📉 Limitations
- Steady-state error up to ~5 mm
- Limited trajectory tracking accuracy
- Limited operating time due to heat generation
