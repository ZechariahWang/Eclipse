![210ZLogo](https://github.com/user-attachments/assets/55f1d4ad-ac78-4a7d-ac7d-db3658863015)

# Eclipse Robotics Library

This is an autonomous robotics framework developed specifically for holonomic and non-holonomic drives. It is a collection of 4+ years of iteration of algorithm improvements and architecture revamps.

The library has been used extensively in regional, national, and international competitions and has earned countless awards. The most notable include winning Canada's largest international robotics tournament sponsored by Encore Canada, Top 16 at the World Championships, and ranking 1st in Alberta. The full list of awards can be found below:

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

## Motivation and Logic
Eclipse was developed by team 210Z, specifically for autonomous portions of the VRC competition. Specifically, it specializes in the 15-second autonomous period of the standard VRC match and the 1-minute programming and driver skills challenge. In addition, it also features custom driver modifications for automated task usage during the op-control period of the match.

Technical specifications include: 
- Latitude and longitudinal Proportional Integral Derivative (PID) Controllers for scenarios in which limited sensor input is available
- Minimal Feedback Control "Approach target position" and "Approach target reference and position" algorithms in the case minimal localization is available
- Odometry Position Localization
- GPS Position Localization
- Scalar Kalman Filters for situations in which obstacles, in which sensor readings may fluctuate and unaccounted forces are introduced
- Bezier Curve generators for path-planning,
- Pure Pursuit Motion Planning for non-linear movements,
- PID Constant Tuners for operator ease
- Holomonic Feedback Control "Approach target position and reference heading"
- Holonomic Pure Pursuit Motion Planning
- Linear Motion Profilers, specifically trapezoidal curves
- LVGL Embedded Graphics, intuitive user interface for operator use
- Autonomous Selector, allows operators to view scripts and datalogs
- AI Python simulations to visualize algorithms and routes, including A*, RRT Pipelines, and more
- Full-stack team tracker web application using React, Express, Node, and MongoDB for scouting opponent statistics


## Framework Usage
1: Clone the repository using ```git clone https://github.com/ZechariahWang/Eclipse-Robot_framework.git```

2: Prepare the VEX ARM-32 Cortex for firmware installation, and configure all robot components, including sensors, radios, etc. This may be done from the ```AssetConfig config``` class for motor and subsystem development.

2: For autonomous control, there are three primary subsections: chassis, modules, and operation systems. These are all divided into their own separate components within the project. Note that certain pieces of logic may require an external module and utility functions, so modifying or customizing logic pieces must be accounted for in the corresponding modules.

3: For LVGL Embedded System Graphics, all logic will be found in ```main.cpp``` or ```Modules/MetricsReturnModule.cpp```. Note that declarations for specific components may be found in other project paths. The current setup of the interface consists of four components: Game, Sensor, Auton, and Misc. Each section displays data about its corresponding section, but may connect to other project parts. The biggest notable example of this is the autonomous selector. 

4: For individual script development, you may either use the Python AI simulations found below, manually input points via trial and error, or preplot routes in real time. The paths used by 210Z are left as templates for how a typical script may be structured. These can be found in ```src/Scripts```.

Library in use: https://www.youtube.com/@zechariah1204

Algorithm Simulations: https://github.com/ZechariahWang/Eclipse-MotionAlgorithm_Simulations

Team Tracker: https://github.com/ZechariahWang/TeamProfiler

## Authors

- [@ZechariahWang](https://github.com/ZechariahWang)

