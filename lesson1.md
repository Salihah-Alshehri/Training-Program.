# Electrical
4 Servo Motors Control Project
🛠️ Hardware Components
 1x Arduino Uno Board  
 4x Micro Servo Motors (SG90)  
 1x Breadboard  
 Jumper Wires   
🔌 Circuit & Wiring Configuration
Power & Ground Connections:
 Power Distribution: The 5V pin from the Arduino connects directly to the positive power rail (+) on the breadboard.  
 Common Ground: The GND pin from the Arduino connects to the negative ground rail (-) on the breadboard.  
 All four servo motors receive power (V_{CC}) and ground (GND) in parallel through the breadboard's power rails.  
Digital Signal Connections:
 Servo 1: Connected to Digital Pin 8 (Gray wire).  
 Servo 2: Connected to Digital Pin 9 (Purple wire).  
 Servo 3: Connected to Digital Pin 10 (Orange wire).  
 Servo 4: Connected to Digital Pin 11 (Brown wire).  
📝 What We Did & System Behavior
1. System Initialization:
Upon powering up the Arduino, all four servo motors are attached to their respective digital PWM pins.  
2. Phase 1 — Sweep Action (First 2 Seconds):
 All four servos synchronously execute a continuous sweeping motion across their angular range.  
 The program tracks elapsed time using ⁠millis()⁠ to ensure the sweep action runs for exactly 2 seconds without freezing execution.  
3. Phase 2 — Hold State (Post 2 Seconds):
 As soon as the 2-second threshold is reached, the sweep action terminates.  
 All four servo motors move to and hold a fixed 90-degree position.  
 The system maintains this held state indefinitely.
(IMG_3639.jpeg)
