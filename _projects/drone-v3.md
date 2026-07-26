---
title: "FPV Drone v3"
description: "TSA \"Safari Rescue\" competition build — indoor obstacle course, no GPS, live payload pickup judged through onboard cameras."
category: "Drone · Flight Control"
status: active
order: 0
tags: [Betaflight, ELRS, FPV, TSA, Payload]
---

## What it is

New 5" freestyle build for the Washington State TSA "2026 Safari Rescue" HS Drone UAV Challenge. Indoor tent course, no GPS lock available, mandatory prop guards, and a payload-pickup task that has to be judged through onboard camera feeds.

## Current state

Reviewing the procurement list against the official rules and getting parts on order. Frame, motors, battery, charger, and props are sourced from the existing inventory; still need the dual-camera vision system (front digital + down analog) and the electromagnet/servo-gripper payload mechanism.

## Build log

<div class="log">

<div class="log-entry">
<div class="log-date">July 26, 2026</div>
<h4>Wrote a white paper on AI-assisted Betaflight configuration</h4>
<p>Bilingual concept paper on using Claude Code as a CLI-based alternative to the Betaflight Configurator GUI — mechanism, capability tiers, safety boundaries, and a proposed workflow. Concept-stage, not yet tested against real hardware.</p>
</div>

<div class="log-entry">
<div class="log-date">July 26, 2026</div>
<h4>Procurement report reviewed against TSA rules</h4>
<p>Went through the procurement report against the WA TSA "Safari Rescue" ruleset. Frame, motors, props, battery, and charger from existing inventory are all keepers. Mapped out what's still needed — dual FPV cameras, electromagnet + servo gripper, mandatory 3D-printed prop guards — and checked every vendor link; the recommended Walksnail HD camera kit turned out to be out of stock. Receipts confirm the frame, motors, batteries, charger, props, and an ELRS receiver + antenna are already in the mail.</p>
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
| Frame | 225mm 5" carbon fiber freestyle |
| FC + ESC | MicoAir H743 V2 |
| Motors | DYS X2807 1300KV x4 |
| Battery | OVONIC 4S 2200mAh 130C |
| Charger | Hiyiton balance charger |
| Radio | ExpressLRS (Nano TX + ER16 RX combo) |
