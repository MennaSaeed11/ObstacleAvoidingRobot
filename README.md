# Robot Control Code with Ultrasonic Sensor

This repository contains Arduino code for controlling a robot with motor drivers, Bluetooth control, and an ultrasonic sensor for obstacle detection.

## Description

This Arduino sketch allows you to control a robot using serial commands sent over Bluetooth. 
The robot has functions for moving forward, backward, turning left, turning right, and stopping. Additionally, it uses an ultrasonic sensor to detect obstacles and avoid collisions.

## Hardware Requirements

- Arduino board (Uno)
- Motor driver module (L298N)
- Bluetooth module (HC-05)
- Motors and wheels for the robot
- Ultrasonic sensor (HC-SR04)

## Commands

The following commands can be sent via serial communication (e.g., Bluetooth terminal):

- `F`: Move forward
- `B`: Move backward
- `L`: Turn left
- `R`: Turn right
- `S`: Stop

## Obstacle Avoidance

The robot uses an ultrasonic sensor to detect obstacles in its path. If an obstacle is detected within 20 cm, the robot will stop, move backward, and then turn right to avoid the obstacle.
