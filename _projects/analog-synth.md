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

Finished prototype works — VCO, audio amplifier, LiPo power, and speaker module all running together. Swapped the pot dial for an analog slider to make note selection easier. Tested by playing Happy Birthday.

## Photos

<div class="img-grid">
  <img src="/assets/img/analog-synth-breadboard.png" alt="Breadboard prototype with discrete VCO circuit">
  <img src="/assets/img/analog-synth-vco-schematic.png" alt="KiCad schematic — Schmitt trigger inverter and VCO">
  <img src="/assets/img/analog-synth-prototype-comparison.png" alt="Breadboard prototype next to finished synth with slider and speaker">
  <img src="/assets/img/analog-synth-protoboard-desk.png" alt="Soldered protoboard with LiPo, slider, and speaker module">
  <img src="/assets/img/analog-synth-final-top.png" alt="Top view of finished synth with slider, LiPo, and speaker">
</div>

## Videos

<div class="video-wrap">
  <video controls playsinline preload="metadata">
    <source src="/assets/video/analog-synth-happy-birthday.mp4" type="video/mp4">
  </video>
</div>

## Build log

<div class="log">

<div class="log-entry">
<div class="log-date">June 7, 2026</div>
<h4>Final test — Happy Birthday on the finished synth</h4>
<p>Added an analog slider for easier note selection in place of the potentiometer dial. Final test with LiPo, synth, and speaker module — works as intended. Played Happy Birthday to confirm.</p>
</div>

<div class="log-entry">
<div class="log-date">June 6, 2026</div>
<h4>Protoboard soldering mostly done</h4>
<p>Finished most of the protoboard soldering for the finished prototype of the synth. Discrete VCO and amp stages coming together on perfboard.</p>
</div>

<div class="log-entry">
<div class="log-date">May 30, 2026</div>
<h4>Finished prototype synth — VCO and audio amplifier</h4>
<p>Completed a working prototype synth with discrete VCO and audio amplifier on the breadboard. Full signal path from oscillator to output confirmed.</p>
</div>

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
