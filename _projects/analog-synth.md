---
title: "Analog Synth"
description: "Custom VCO built from discrete parts — no ICs, just transistors, resistors, and capacitors. CAD and build a matching speaker next."
category: "Circuits · Analog Audio"
status: active
order: 5
tags: [VCO, KiCad, Transistors, Analog, Speaker]
---

## What it is

An analog synthesizer voice built entirely from bare components — no oscillator chips, no op-amp ICs. The core is a discrete voltage-controlled oscillator: Schmitt trigger inverter stages from transistors, timing set by resistors and capacitors.

Next step is CADding and building a speaker enclosure to match it.

## Current state

Ongoing — breadboard prototype is running. VCO schematic is laid out in KiCad; tuning the Schmitt trigger stage and working toward a stable, controllable pitch. Speaker design not started yet.

## Photos

<div class="img-grid">
  <img src="/assets/img/analog-synth-breadboard.png" alt="Breadboard prototype with discrete VCO circuit">
  <img src="/assets/img/analog-synth-vco-schematic.png" alt="KiCad schematic — Schmitt trigger inverter and VCO">
</div>

## Build log

<div class="log">

<div class="log-entry">
<div class="log-date">May 24, 2026</div>
<h4>VCO schematic drawn in KiCad</h4>
<p>Laid out the discrete Schmitt trigger inverter and voltage-controlled oscillator — 2N2222 stages, timing cap and pot, no ICs. Ready to iterate against the breadboard build.</p>
</div>

<div class="log-entry">
<div class="log-date">May 23, 2026</div>
<h4>Breadboard VCO prototype live</h4>
<p>Discrete Schmitt trigger inverter oscillating on the breadboard. No ICs — just 2N2222s, passives, and a pot for frequency control. Next: tighten up the waveform and start the speaker CAD.</p>
</div>

</div>
