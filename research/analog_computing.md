---
date: 2026-04-18
tags: [computing, analog, hardware, history]
sources:
  - "Bush, Vannevar — Differential Analyzer (1930s)"
  - "Prigogine, Ilya — dissipative structures and analog systems"
  - "Antikythera Mechanism research"
---

# Analog Computing

## Core Principle

The physical medium IS the computation. A voltage of 3.7V represents the number 3.7. A gear rotation of 47 degrees represents 47 degrees. The physics does the math directly.

```
Mathematical operation    Physical implementation
─────────────────────    ──────────────────────
Addition                  Sum two voltages
Integration               Charge a capacitor
Multiplication            Potentiometer ratio
Differential equation     Wire up a matching circuit
```

Computation happens **continuously** and **in parallel** — every component computes simultaneously. No clock, no steps, no sequence. The circuit reaches its answer the way water finds its level — by settling into physical equilibrium.

## History

**Antikythera Mechanism (~100 BC)** — ancient Greek device with interlocking bronze gears predicting astronomical positions, eclipses, and calendar cycles. Found in a shipwreck in 1901. Continuous gear rotation represents continuous celestial motion. The physics of the gears mirrors the physics of the sky.

**Slide Rule (1620s)** — two logarithmic scales that slide against each other. Multiplication = physically adding distances on logarithmic scales. The physical operation IS the mathematical operation. Used by every engineer until the 1970s. Apollo missions were calculated partly with slide rules.

**Kelvin's Tide Predictor (1876)** — mechanical analog computer summing harmonic functions using pulleys and gears to predict tides. Physical motion of gears directly represented mathematical summation of wave functions.

**Vannevar Bush's Differential Analyzer (1930s)** — room-sized mechanical analog computer solving differential equations. Rotating shafts, wheels, disc integrators. Set up the physical configuration to match the equation, turn the crank, machine traces the solution. Used for ballistics and engineering.

**WWII Fire Control Computers** — analog computers on warships calculating firing solutions in real-time. Input: ship speed, target speed, wind, range. Output: where to point the gun. Gears, cams, servomotors. Had to work in real-time — analog was the only option fast enough.

**Electronic Analog Computers (1940s-1970s)** — replaced gears with electronic components. Operational amplifiers, capacitors, resistors representing mathematical operations. NASA used analog computers extensively in the early space program — could simulate rocket trajectories in real-time by building circuits whose behavior matched the physics.

## Strengths

- Energy efficient — physics does the math, no encoding overhead
- Naturally parallel — all components compute simultaneously
- Excellent for continuous problems — differential equations, simulation, optimization
- Real-time — no clock cycles, answer emerges as fast as the physics settles
- No von Neumann bottleneck — computation and "memory" (component values) are co-located

## Weaknesses

- Noise accumulates through computation — can't separate signal from noise
- Limited precision — constrained by component quality, thermal noise, manufacturing variation
- Hard to reprogram — typically designed for one class of problem
- Doesn't scale like digital — components don't shrink according to Moore's Law
- Results vary with temperature, component aging, manufacturing differences
- No error correction — once a value drifts, it's gone

## The Brain Is an Analog Computer

Neurons pass continuous graded potentials. Synaptic weights are continuous. No discretization between layers. The brain tolerates noise through redundancy, averaging, and computations robust to small perturbations. This is why the brain achieves 10,000x better energy efficiency than digital hardware.

See also: [[digital_computing]] [[analog-vs-digital-and-the-middle-ground]] [[brain]] [[energy-cost-of-intelligence]]
