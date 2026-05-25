---
title: "3-sensor ultrasonic array working without cross-echo"
project: "Mini Wheeled Robot"
date: 2026-05-22
---

Staggered trigger timing with Timer1 interrupts finally works. 60ms gap between each sensor's trigger pulse prevents inter-sensor echo interference. All three HC-SR04s reading stable within ±1cm. Next: write the avoidance logic that uses all three readings together.
