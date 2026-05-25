---
title: "Custom ESC"
description: "Designing a brushless motor ESC from scratch — gate driving, BEMF sensing, commutation."
category: "Circuits · Motor Control"
status: paused
order: 3
tags: [BLDC, KiCad, MOSFET, STM32]
---

## What it is

A from-scratch brushless ESC (Electronic Speed Controller). Most people buy these. I want to understand every transistor.

The goal: 20A continuous, 3S LiPo input, sensorless BLDC commutation using back-EMF zero-crossing detection.

## Current state

Paused — waiting on IR2101 gate driver ICs from order. Should arrive next week.

PCB layout is ~80% done in KiCad. The low-side MOSFET bootstrap circuit gave me grief — figured out I need a longer dead time than I expected to prevent shoot-through.

## What I've learned so far

- MOSFET gate drive is more subtle than I thought. The gate capacitance means you need real drive current, not just logic-level signals.
- Shoot-through is a real concern. Even 10ns of overlap between high and low side = dead FETs.
- Bootstrap capacitors need to fully charge before the first PWM cycle — sequencing matters.

## Build log

<div class="log">

<div class="log-entry">
<div class="log-date">May 8, 2026</div>
<h4>Bootstrap circuit redesigned</h4>
<p>Original design had bootstrap cap too small (100nF). Calculated minimum charge needed for gate drive at 20kHz switching — upped to 470nF. Also added a 10Ω gate resistor to limit dI/dt and reduce EMI.</p>
</div>

<div class="log-entry">
<div class="log-date">Apr 28, 2026</div>
<h4>Schematic complete, starting layout</h4>
<p>Full schematic done: 3-phase bridge (6x IRF540N), IR2101 gate drivers x3, current sense via shunt, STM32F030 for commutation control. Starting PCB layout.</p>
</div>

</div>
