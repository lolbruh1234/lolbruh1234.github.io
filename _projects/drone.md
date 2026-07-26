---
title: "FPV Drone v2"
description: "5\" freestyle FPV build from scratch — frame, PDB, firmware, the whole thing."
category: "Drone · Flight Control"
status: active
order: 1
tags: [STM32, Betaflight, LiPo, BLHeli]
---

## What it is

5" freestyle FPV drone, built from scratch. Not a kit — I sourced every component, designed the power distribution board in KiCad, and configured Betaflight from defaults.

## Current state

Fighting yaw oscillation at high throttle. P term on yaw is causing a noticeable wobble above ~60% throttle. Trying to isolate whether it's a mechanical resonance issue (props, motor mounts) or a pure PID tuning problem.

## Build log

<div class="log">

<div class="log-entry">
<div class="log-date">May 25, 2026</div>
<h4>Blackbox analysis — yaw P overshoot</h4>
<p>Pulled Blackbox logs and graphed the yaw gyro vs. setpoint. Clear overshoot pattern consistent with P being too high. Dropping yaw P from 45 → 35 and re-testing tomorrow.</p>
</div>

<div class="log-entry">
<div class="log-date">May 18, 2026</div>
<h4>First real flight — maiden success</h4>
<p>First outdoor flight. Hovers stable, pitch/roll feel decent. Yaw is twitchy but flyable. Burned a motor mount on landing #3. Reprinted overnight.</p>
</div>

<div class="log-entry">
<div class="log-date">May 10, 2026</div>
<h4>PDB assembled and tested</h4>
<p>Custom PDB soldered. All 4 ESC pads confirmed at 16.8V under load. Current sense resistors reading correctly through ADC. Ready for motor mount.</p>
</div>

</div>

## Photos

<!-- Drop your photos into /assets/img/ and reference them like this: -->
<!-- <div class="img-grid">
  <img src="/assets/img/drone-frame.jpg" alt="Frame assembly">
  <img src="/assets/img/drone-pdb.jpg" alt="PDB soldered">
  <img src="/assets/img/drone-maiden.jpg" alt="First flight">
</div> -->

## Videos

<!-- Paste a YouTube embed like this: -->
<!-- <div class="video-wrap">
  <iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID" allowfullscreen></iframe>
</div> -->

## Parts list

| Part | Model |
|------|-------|
| Frame | 5" stretch X |
| FC | F7 (STM32F7) |
| ESC | 4-in-1 35A BLHeli_32 |
| Motors | 2306 2450kv |
| Camera | Runcam Phoenix 2 |
| VTX | Rush Tank 2W |
