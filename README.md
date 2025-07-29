![210ZLogo](https://github.com/user-attachments/assets/55f1d4ad-ac78-4a7d-ac7d-db3658863015)

# Eclipse 2021-2024 Library

Autonomous Code framework developed by 210Z. 

Library in use: https://www.youtube.com/@zechariah1204

Algorithm Simulations: https://github.com/ZechariahWang/Eclipse-MotionAlgorithm_Simulations

Team Tracker: https://github.com/ZechariahWang/TeamProfiler

- Div Top 16 World Championships
- 7x World Championship Qualified
- 7x Regional Tournament Champions
- 6x Regional Tournament Finalists
- 9x Design, Skills, Sportsmanship, Judges, Innovate Awards
- 2x International Tournament Champion
- 1x Provincial Champion
- 2x Excellence Award
- 1x Think Award
- Western Mechatronics 2024 Excellence in Programming Award
- Calgary Stampede Agriculture Technology 2nd Place

Contains Proportional Integral Derivative (PID) Controllers, Feedback Control MTP and MTRP, Kalman Filters, Bezier Curve Path Planners, Pure Pursuit Path Trackers, PID Constant Tuners, Odometry Position Localization, Holomonic Feedback Control MTP, Linear Motion Profilers with Inverse Kinematics, LVGL Integrated Graphics, Autonomous Selector, Metrics Modular Control.

## Project Usage
1: Install the package from this repository using ```git clone https://github.com/ZechariahWang/Eclipse-Robot_framework.git```

2: For autonomous control, there are three main components: PID Controller, Odometry Logic, and Algorithm Logic. These are all divided into their own seperate components within the project. Note that certain pieces of logic may require external module and utility functions.

3: For LVGL Embedded System Graphics, all logic will be found in ```main.cpp``` in the ```initialize``` function. Note that declarations for specific components may be found in other project paths. The current setup of the interface is in 4 components: Game, Sensor, Auton, Misc. Each section displays data about its corresponding section but may connect to other project parts. The biggest notable example of this is the autonomous selector.

## Authors

- [@ZechariahWang](https://github.com/ZechariahWang)

