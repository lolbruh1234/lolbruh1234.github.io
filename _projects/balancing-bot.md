---
title: "Self-Balancing Bot"
description: "Two-wheeled inverted pendulum robot — IMU + PID + custom PCB."
category: "Robotics · Control Theory"
status: planning
order: 4
tags: [MPU-6050, PID, TB6612, KiCad]
---

## What it is

Classic two-wheeled self-balancing robot, but done properly. Not an Arduino shield stack — a custom single PCB with integrated IMU, motor drivers, and MCU.

## Why I'm building it

Self-balancing robots are a great control theory exercise. The math is clean enough to reason about but hard enough that bad PID tuning is immediately obvious (it falls over).

## Plan

**Hardware:**
- STM32F103 (Blue Pill compatible)
- MPU-6050 IMU (accelerometer + gyroscope, I²C)
- TB6612FNG dual motor driver
- 2x 6V DC gear motors with encoders
- Single 2-layer PCB, designed in KiCad

**Firmware:**
- Complementary filter for IMU fusion (gyro drift + accel noise compensation)
- PID control loop at 500Hz
- UART debug output for real-time PID tuning

## Status

Currently in PCB design. Schematic is done, laying out the board now. Keeping it small: targeting 80mm × 60mm so it fits between the wheels cleanly.
