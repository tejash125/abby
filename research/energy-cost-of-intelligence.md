---
date: 2026-04-06
tags: [energy, efficiency, hardware, brain, neuromorphic, economics, thermodynamics]
sources:
  - "Landauer, R. — Irreversibility and Heat Generation in the Computing Process (1961)"
  - "Intel Loihi 2 neuromorphic processor specifications"
  - "IBM TrueNorth chip specifications"
  - "BrainScaleS project, University of Heidelberg"
  - "SpiNNaker project, University of Manchester"
---

# Energy Cost of Intelligence

## The Cost Chain

Every AI computation has a physical cost chain:

```
Problem to solve
  → Computation required
    → Electricity consumed
      → Energy source exploited
        → Thermodynamic cost (entropy increase)
```

The price of AI work is ultimately anchored to the price of electricity. Everything else — hardware, cooling, networking, salaries — matters, but electricity is the floor.

## Electricity Pricing Is Political, Not Physical

Electricity is not a single global market. The same kWh costs ~$0.03 in parts of the Middle East or Scandinavia and ~$0.35 in Germany or California. A 10x difference for the same physical thing.

Price is determined by:
- **Generation cost** — varies by source (coal/gas vs nuclear vs solar/wind vs hydro)
- **Transmission and distribution** — often the largest chunk of the bill, not generation
- **Regulatory and market structure** — subsidies, taxes, monopolies, deregulation
- **Time-of-use** — 3 AM electricity costs less than 6 PM electricity

The cost of AI work depends enormously on where the data center sits.

## The AI-Electricity Demand Spiral

AI training compute scales ~4x per year. Hardware efficiency improves ~2x every 2-3 years. Net result: total energy consumption grows exponentially.

- Data center electricity demand projected to double or triple by 2030
- New data centers being denied grid connections in some regions
- Microsoft, Google, Amazon signing nuclear power deals
- Increased demand raises prices for everyone

AI's own success makes it more expensive. More capability → more demand → more infrastructure → higher energy costs → higher AI costs.

## The Human Replacement Crossover

Currently: AI cost per task << human cost per task (for many tasks).

But if electricity costs rise significantly, the gap narrows. For some tasks in some regions, a human willing to work cheaply becomes more cost-effective than the computation. The crossover isn't fixed — it moves with electricity price, hardware efficiency, and wage levels. It's a dynamic equilibrium.

## What If Energy Becomes Cheap?

**Fusion:** Near-unlimited fuel, no carbon, high energy density. Electricity becomes extremely cheap globally. AI cost floor drops dramatically. The economic advantage of AI over human labor widens. Geographic arbitrage disappears.

**Radical solar + storage:** Near-zero marginal cost. Equatorial countries become energy-rich. Energy poverty could be eliminated.

If energy becomes 100x cheaper, you don't just get the same AI cheaper — you get AI trained with 100x more compute, which means qualitatively different capability. The constraint isn't just price; it's what the price makes possible.

## The Thermodynamic Floor

Even with free electricity, computation can never be truly free. **Landauer's principle**: erasing one bit of information requires minimum energy of kT ln 2 (~3 × 10⁻²¹ joules at room temperature).

Current computers operate ~10⁶ times above this limit. Enormous room for efficiency improvement — but the floor is non-zero. Organizing information always increases entropy somewhere, and that has an energy cost.

Even with unlimited free electricity, heat dissipation becomes the bottleneck. Cooling, not generation, becomes the constraint.

## Brain vs AI: The Efficiency Gap

| Metric | Brain | Current AI Hardware |
|---|---|---|
| Power | ~20W | ~700W per GPU (clusters use thousands) |
| Ops per watt | ~10¹⁵-10¹⁶ | ~10¹²-10¹³ |
| Efficiency gap | — | ~1,000-10,000x worse |

The brain handles vision, language, reasoning, motor control, emotion, memory — all simultaneously on 20 watts. Training a frontier LLM uses 50-100 GWh (a small city's annual consumption) and produces a system that does language well but nothing else.

## Why the Brain Is So Efficient

Not just better engineering — a fundamentally different computational paradigm:

**Co-located memory and compute:** The synapse IS both memory and compute element. No von Neumann bottleneck. In GPUs, moving data between memory and compute uses 100-1000x more energy than the computation itself. Most GPU electricity goes to data movement, not computing.

**Sparse activation:** Only ~1-5% of neurons fire at any given moment. GPUs compute densely — every core runs every cycle whether useful or not.

**Event-driven, not clock-driven:** Neurons fire only when they have something to communicate. GPUs run on a global clock — every transistor transitions every cycle.

**Analog, not digital:** Continuous voltages, no energy spent maintaining sharp 0/1 signal levels. Low precision but noise-tolerant by design. Digital computation enforces discrete signal levels at 16-32 bit precision — energetically expensive and mostly overkill.

**3D structure:** Dense 3D network, short average wiring distance. Chips are essentially 2D — longer interconnects, more energy for signal transmission.

**600 million years of optimization:** Evolution under extreme metabolic pressure ruthlessly optimized neural computation toward thermodynamic efficiency.

## Hardware Efficiency Trend

- 2012 (AlexNet era): ~10⁹ FLOPS/W
- 2016 (TPU v1): ~10¹¹ FLOPS/W
- 2020 (A100): ~10¹² FLOPS/W
- 2024 (H100/B200): ~10¹²-10¹³ FLOPS/W
- Brain: ~10¹⁵-10¹⁶ FLOPS/W

Roughly 10x improvement every 5-7 years. At this rate, reaching brain-level efficiency: 15-25 years — if the trend continues. But Dennard scaling ended ~2006, Moore's Law is slowing, and each further shrink is exponentially more expensive ($20B+ per new fab).

## Neuromorphic Computing

Projects attempting to replicate brain architectural advantages:

- **Intel Loihi 2** — spike-based, event-driven, ~1000x more energy efficient than GPUs for certain tasks
- **IBM TrueNorth** — 1M neurons, 256M synapses, ~70mW, real-time video classification at brain-like power
- **BrainScaleS (Heidelberg)** — mixed-signal analog/digital, runs 1000x faster than biological real-time
- **SpiNNaker (Manchester)** — massively parallel spiking neural network simulator, 1M ARM cores

All early stage. None can do what transformers do. The fundamental problem: we know how to build brain-like hardware and capable AI software, but the algorithms (backpropagation, attention, transformers) are designed for dense, synchronous, digital hardware and don't map onto neuromorphic chips.

## The Fundamental Question

Is the efficiency gap due to:

**(a) Engineering gap** — need better chips, more R&D. Gap will close incrementally. Industry's default assumption.

**(b) Wrong paradigm** — digital, synchronous, von Neumann computing is the wrong substrate. No amount of engineering closes a 10,000x gap if the architecture is wrong. Need a paradigm shift.

**(c) Evolutionary optimization** — 600 million years of optimization under extreme energy pressure. Can't replicate that timeline through engineering.

**(d) Meaningless comparison** — brain and GPUs do fundamentally different things. Comparing FLOPS is like comparing a bird's wing to a propeller by measuring RPM.

Probably all four, with (b) most important for Abby. If the goal is brain-like intelligence at brain-like efficiency, the current paradigm may be a dead end — not because the chips are slow, but because the architecture is wrong at every level.

The brain isn't just a more efficient computer. It's a different kind of machine that happens to also compute.

See also: [[brain]] [[analog_computing]] [[digital_computing]] [[information_processing]] [[entropy-is-not-complexity]] [[inherited-tools]]
