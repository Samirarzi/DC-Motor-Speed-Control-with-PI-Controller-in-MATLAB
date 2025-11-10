#DC Motor Speed Control Using 3-Phase Fully Controlled Thyristor Converter (6-Pulse) in MATLAB/Simulink

📘 Overview

This project simulates a separately excited DC motor driven by a three-phase fully controlled thyristor converter (6-pulse converter).
The main objective is to control the speed of the DC motor using PI controllers for both the armature current and the motor speed.
The system is modeled and simulated entirely in MATLAB/Simulink, demonstrating the closed-loop control structure for accurate speed regulation.

⚙️ System Description

The overall model consists of:

Three-phase AC source feeding the thyristor converter.

6-pulse controlled rectifier converting AC to DC with variable output voltage.

Separately excited DC motor used as the load.

Dual-loop PI control system:

Inner loop controls the armature current.

Outer loop controls the motor speed.


Pulse generator that produces thyristor firing signals based on the control angle (α).


🧩 Model Components

Speed Reference Input (ω_ref) – desired motor speed.

PI Controller (Speed Loop) – minimizes the error between ω_ref and actual speed.

PI Controller (Current Loop) – regulates the armature current.

Firing Angle Control (α) – computed using the control voltage output.

6-Pulse Converter – generates the DC voltage applied to the motor.

DC Motor Block – simulates the electromechanical dynamics.


📊 Outputs

The simulation provides:

Motor speed (rpm)

Reference speed (rpm)

Armature current (Ia)

Electromagnetic torque (Te)

Converter output voltage (Va)


🚀 Simulation Details

Environment: MATLAB/Simulink

Simulation type: Discrete

Sample time: 1e-5 seconds

Control type: Closed-loop PI speed and current control


📈 How to Run

1. Open the .slx file in MATLAB/Simulink.


2. Set the desired reference speed and motor parameters.


3. Run the simulation.


4. Observe waveforms for speed, current, and torque.



🧠 Key Learning Outcomes

Understanding the interaction between converter and DC motor dynamics.

Implementation of nested PI controllers for speed and current regulation.

Generation of thyristor firing pulses based on control voltage.

