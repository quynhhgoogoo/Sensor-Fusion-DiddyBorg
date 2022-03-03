# Sensor-Fusion-DiddyBorg
Project Work for Sensor Fusion course at Aalto University

## Introduction

The aim of this project is to develop an algorithm for tracking an autonomous robot by using a set of sensors. 

The robot, a DiddyBorg rover-type robot, is programmed to follow a black line inside a closed area surrounded by walls. The robot is equipped with an inertial measurement unit (IMU), which is a combination of accelerometer, gyroscope, and magnetometer. In addition to the IMU, the robot is also equipped with an infra red detector, a motor controller, and a camera module. 
The IMU will measure the acceleration as well as the angular rate of the robot from three orthogonal body axis. 
The accelerometer measurements and the gyroscope measurements (angular velocity) from IMU are combined to obtain the acceleration in the inertial frame. The velocity and the position of the robot are then readily obtained by integration of the acceleration. However, as time increases, the error will be accumulated, and hence the deviation from the actual position grows. The camera system will detect several predefined rectangles, which contain unique QR codes with known position attached in the wall. This measurements can be used to correct the position estimate obtained by twice integration.

The sensors are connected to the main computer which is a Raspberry Pi. The Raspberry Pi is responsible to handle all sensor measurement preprocessing and logging. It can also be used to transfer the recorded measurements data to other means.

The project consists of two parts. In the first part, we develop and verify the sensor model for the IMU and camera system. This includes the following steps:
- Derivation of the sensor model
- Estimation of the model parameters



###  Running `Sensor Modeling.ipynb`
Required Python packages are `numpy, pandas, matplotlib, statistics`
