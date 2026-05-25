---
title: "Mini Wheeled Robot"
description: "Started as a kit, now fully custom firmware and sensor fusion."
category: "Robotics · Embedded"
status: active
order: 2
tags: [Arduino, HC-SR04, L298N, C++]
---

## What it is

Two-wheel differential drive robot. Bought a basic kit to learn the mechanics, then threw out the example code and rewrote everything. Currently adding an ultrasonic sensor array for proper obstacle avoidance (not just "stop when something is close").

## Current state

Wiring up 3 HC-SR04 sensors (front, front-left, front-right) to build a simple spatial map. The challenge is timing — you can't fire all three at once or they echo off each other. Implementing staggered triggers with interrupt-driven echo capture.

## Build log

<div class="log">

<div class="log-entry">
<div class="log-date">May 22, 2026</div>
<h4>Staggered ultrasonic timing working</h4>
<p>Got all 3 sensors reading without cross-echo. Trick: 60ms gap between each trigger, use Timer1 interrupts to capture echo pulse width without blocking loop(). Readings are stable within ±1cm.</p>
</div>

<div class="log-entry">
<div class="log-date">May 15, 2026</div>
<h4>Rewrote motor control — no more analogWrite jitter</h4>
<p>Default analogWrite was causing jitter at low speeds because of its 490Hz PWM. Switched to Timer2 direct register manipulation at 20kHz. Motors are now smooth at 15% duty cycle.</p>
</div>

</div>

## Photos

<!-- <div class="img-grid">
  <img src="/assets/img/robot-wiring.jpg" alt="Sensor wiring">
  <img src="/assets/img/robot-top.jpg" alt="Top view">
</div> -->
