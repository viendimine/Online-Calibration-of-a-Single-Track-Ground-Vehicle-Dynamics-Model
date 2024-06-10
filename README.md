# ST-VIO :Online Calibration of a Single-Track Ground Vehicle Dynamics Model by Tight Fusion with Visual-Inertial Odometry
Haolong Li1 and Joerg Stueckler1

## Objective:
ST-VIO (Single-Track Visual Inertial Odometry) is a novel approach designed to enhance the navigation and motion estimation capabilities of wheeled mobile robots. This system tightly integrates a single-track dynamics model with visual inertial odometry (VIO) to improve the accuracy of motion predictions and control actions for navigation planning.

## Single Track Dynamics Model

![Single_Track_Dynamics_Model](https://github.com/vishapraj/Online-Calibration-of-a-Single-Track-Ground-Vehicle-Dynamics-Model/assets/126682925/7508b2e4-5d7c-42f5-84bc-acdbb868214c)

The Single Track Dynamics Model, also known as the Bicycle Model or the Rigid Rider Model, is a widely used model in the field of vehicle dynamics for analyzing and predicting the motion and stability of two-wheeled vehicles, such as motorcycles, bicycles, and other similar vehicles.
The model simplifies the vehicle by representing it as a single rigid body with two wheels, one in the front and one in the rear. The front wheel is assumed to be steerable, while the rear wheel is fixed. The model assumes that the vehicle moves in a plane, neglecting any vertical motion or roll dynamics.

## Visual Inertial Odometry

https://github.com/vishapraj/Online-Calibration-of-a-Single-Track-Ground-Vehicle-Dynamics-Model/assets/126682925/80659e80-9e5e-4312-a001-2850e927c79e

Visual Inertial Odometry (VIO) is a technique used in robotics and autonomous systems for estimating the pose (position and orientation) of a moving platform, such as a robot, vehicle, or drone, by fusing data from visual sensors (e.g., cameras) and inertial sensors (e.g., accelerometers and gyroscopes).Here's how VIO works:
### 1.Visual Odometry(VO):-
* Visual sensors (cameras) are used to track features (e.g., corners, edges) in the environment across consecutive frames.
* By analyzing the motion of these features, the system can estimate the relative motion of the platform between frames, providing incremental pose updates.
* However, VO is prone to drift over time due to accumulated errors and is sensitive to rapid motions or lack of distinguishable features.
### 2.Inertial Measurements:-
* Inertial sensors (accelerometers and gyroscopes) provide linear acceleration and angular velocity measurements, respectively.
* These measurements can be integrated to estimate the platform's pose, but they suffer from unbounded drift due to sensor biases and integration of noise over time.
### 3.Sensor Fusion:-
* VIO combines the strengths of both visual and inertial sensors by fusing their data in a tightly coupled manner.
* The visual measurements provide absolute pose updates to correct the drift in the inertial measurements, while the inertial measurements help maintain pose estimates during rapid motions or when visual features are unavailable.
