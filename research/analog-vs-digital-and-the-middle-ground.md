---
date: 2026-04-18
tags: [computing, analog, digital, hardware, architecture, neuromorphic, foundational]
sources:
  - "IBM Analog AI research"
  - "Mythic AI — analog neural network inference"
  - "Rain Neuromorphics — memristor-based analog AI"
  - "BrainScaleS project, University of Heidelberg"
---

# Analog vs Digital and the Middle Ground

## The Core Distinction

**Analog:** the physical medium IS the computation. A voltage of 3.7V represents 3.7. Physics does the math. Continuous, parallel, no encoding overhead.

**Digital:** the physical medium ENCODES symbols. A high voltage = "1", low = "0". Symbols are manipulated by logic rules. Discrete, sequential, layered abstraction between physics and math.

The abstraction that makes digital inefficient is the same abstraction that makes it universal.

## Why Not Keep Continuous Values? (The Middle Ground Question)

The natural question: transistors produce continuous voltage outputs. Why force them into 0/1? Why not pass 0.37V as 0.37V to the next stage and keep the information?

### Why It's Hard

**Noise accumulation — the fundamental problem:**
- Digital: signal of 0.85V (meant to be 0.9V "1") → still clearly "1" → regenerate to 0.9V → clean signal, no damage
- Analog: signal of 0.370V picks up noise → 0.373V → next stage adds noise → 0.376V → after 100 stages, value has drifted by unknowable amount
- Digital signals can be cleaned at every step. Analog noise is permanent and cumulative
- Once noise corrupts a continuous value, signal and noise are inseparable

**Component variation:** Two transistors on the same chip aren't identical. Manufacturing variation. Digital: doesn't matter, both agree on "high" vs "low." Analog: same input gives slightly different outputs.

**Precision vs physics:** Distinguishing 0.370V from 0.371V requires resolving 1mV. At that scale, thermal noise (Johnson-Nyquist noise from random electron motion) is significant. This is fundamental physics, not engineering. Digital only needs to distinguish "high" from "low" — hundreds of millivolts apart.

**Error correction:** Digital has parity bits, checksums, ECC. Detect error, fix it. Analog has no equivalent — once a value drifts, no way to detect or correct without knowing what it should have been.

### Why Neural Networks Change Everything

Neural networks are inherently **noise-tolerant**:
- Models trained with 32-bit weights work nearly as well quantized to 8-bit, 4-bit, sometimes binary
- Redundancy in networks means small perturbations don't change outputs significantly
- The computation doesn't need high precision — "roughly 0.37" is good enough

This means the primary objection to analog computing (noise accumulation) **doesn't apply to the main workload we care about now.**

### The Brain Does Exactly This

The brain keeps continuous values and passes them forward:
- Neurons operate with continuous graded potentials
- Synaptic weights are continuous, not binary
- Output of one neuron feeds directly into the next — no discretization
- Noise is tolerated through redundancy, averaging, and robust computation
- This is why the brain is 10,000x more energy efficient

## The Middle Ground Being Built Right Now

### In-Memory Analog Computing

Store neural network weights as analog values in memory cells. Pass input as voltage. Physics does the math:

- Output current = input voltage × stored conductance = **multiplication by physics**
- Sum currents from many cells = **dot product by physics**
- The core neural network operation (matrix multiply) happens without binary conversion, without data movement

### Who's Doing It

| Company/Lab | Approach |
|---|---|
| IBM Analog AI | Phase-change memory for analog matrix multiplication |
| Mythic AI | Flash memory cells storing analog weights |
| Rain Neuromorphics | Memristor-based analog AI chip |
| Aspinity | Analog ML at the sensor edge |
| BrainScaleS (Heidelberg) | Mixed-signal: analog neural dynamics, digital communication |

### The Emerging Architecture: Analog Compute, Digital Communicate

```
Analog domain                          Digital domain
─────────────                          ──────────────
Matrix multiplication (physics)   →    Results converted to digital
Dot products (current summation)  →    Sent between chips digitally
Activation functions (circuits)   →    Error correction applied
                                  →    Stored in digital memory
                                  ←    Next layer's input converted to analog
```

Heavy math in analog — fast, parallel, efficient. Digital for communication, error correction, storage. Best of both worlds.

### Multi-Level Cells Already Exist

NAND flash memory already keeps more than just 0/1:
- SLC: 1 bit per cell (high/low)
- MLC: 2 bits per cell (4 voltage levels)
- TLC: 3 bits per cell (8 levels)
- QLC: 4 bits per cell (16 levels)

This is the middle ground in practice — keeping more of the analog range. Trade-off: more levels = harder to distinguish = more errors = slower reads = shorter lifespan.

## Why This Wasn't Done Earlier

1. **General-purpose computing needs precision.** Accounting, databases, text — need exact answers. 0.370 must stay 0.370 through a billion operations. Analog can't guarantee this.
2. **Moore's Law only applied to digital.** Transistors shrink. Analog components don't scale the same way. Digital got exponentially cheaper.
3. **No killer application needed it.** Until neural networks. Matrix multiplication, noise tolerance, massive parallelism — exactly what analog does well and what neural networks need.

The middle ground wasn't viable before because there was no workload that needed it. Now there is.

## The 70-Year Irony

Started with analog → abandoned for digital (more flexible, scalable) → built neural networks on digital hardware that simulate analog computation → going back to analog hardware to run them efficiently. A 70-year detour to arrive back where we started, but knowing why.

## Relevance to Abby

If:
- The brain computes in continuous analog values
- Neural networks are mathematically continuous operations
- Analog hardware runs neural computation 100-1000x more efficiently
- Noise tolerance of neural networks makes analog viable

Then the path for Abby might not be "better digital hardware" but the right analog/mixed-signal substrate — where the physics does the computation instead of encoding everything into symbols.

See also: [[analog_computing]] [[digital_computing]] [[brain]] [[energy-cost-of-intelligence]] [[inherited-tools]]
