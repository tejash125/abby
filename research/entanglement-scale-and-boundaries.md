---
date: 2026-05-12
tags: [physics, quantum, entanglement, scale, biology, foundational]
sources:
  - "Kotler et al. — Direct observation of deterministic macroscopic entanglement, Science (2021)"
  - "Mercier de Lépinay et al. — Quantum mechanics-free subsystem with mechanical oscillators, Science (2021)"
  - "Zhang, Xu et al. — Cryogenic dual-ion trap entangled state storage, Tsinghua University"
  - "Nature Photonics — Single-qubit quantum memory exceeding 10-minute coherence time (2018)"
  - "Nature Communications — Quantum entanglement lasts 600x longer in dark states (2025)"
  - "Nature — Long-lived entanglement of molecules in magic-wavelength optical tweezers (2025)"
---

# Entanglement: Scale and Boundaries

## The macroscopic entanglement experiment (aluminum drums)

### What are the drums?

Two thin sheets of aluminum patterned onto a sapphire chip — like tiny trampolines. Each about 20 micrometers long (the width of a red blood cell), weighing about 70 picograms. Each contains **several billion atoms.** The two drums vibrate at different speeds (11 million and 16 million times per second) so researchers can tell them apart.

### The environment

The setup sits inside a refrigerator cooled to below 0.01 degrees above absolute zero. Two reasons:
- At room temperature, random thermal vibration drowns out quantum effects. Near absolute zero, the drums are nearly perfectly still — only quantum-level vibrations remain.
- At this temperature, aluminum becomes superconducting (conducts electricity with zero resistance), which matters because the measurement depends on clean electrical signals.

### How the drums are coupled

Underneath each drum is a flat metal plate. Drum + plate form a sandwich with a gap. When the drum vibrates, the gap changes, which changes how much electrical charge the sandwich can hold. Physical vibration becomes an electrical signal.

Both drums connect to the same electrical circuit — a loop including a large spiral of wire. This circuit has its own natural frequency (about 6 billion oscillations per second). The drums and circuit are coupled: vibrations affect the electrical signal, and electrical signals affect the drums. The circuit is the bridge between the two drums.

### How entanglement was created

Precisely timed pulses of microwave energy are sent into the circuit:

1. **First pulse** hits drum 1 at a specific frequency → creates a single unit of vibration in drum 1 AND a single unit of microwave energy in the circuit, linked by conservation laws. Drum 1's vibration and the circuit's signal are now entangled.

2. **Second pulse** hits drum 2 at a different frequency → transfers the circuit's microwave energy into a vibration in drum 2.

After both pulses: drum 1 has a vibration, drum 2 has a vibration, and the two are entangled. The circuit acted as intermediary — carried the entanglement from drum 1 to drum 2, then got out of the way.

### How they verified it's entanglement, not just two connected things vibrating together

Two drums connected by the same circuit could easily be correlated classically — like two pendulums hanging from the same beam. That's not entanglement. The difference: **how tight the correlations are.**

For any individual system, there's a minimum uncertainty — you can't know both position and momentum perfectly. For two independent or classically-correlated systems, the combined uncertainty has a minimum threshold it can't go below.

For entangled systems, the correlations are **tighter than this threshold allows.** When they measured drum 1's position, they could predict drum 2's position more precisely than any non-entangled explanation permits. Positions correlated (moved same direction), momenta anti-correlated (moved opposite directions) — and the precision exceeded the classical limit by an order of magnitude (about 10x beyond the threshold).

Same logic as Bell tests: there's a mathematical ceiling for correlations between systems with independent properties. Exceeding it = entanglement confirmed.

## How long entanglement lasts

| What was entangled | Duration | When |
|---|---|---|
| Aluminum drums (billions of atoms) | Microseconds (millionths of a second) | 2021 |
| Photons stored in a crystal | ~2 microseconds | 2023 |
| Molecules in controlled traps | Milliseconds (thousandths of a second) | 2025 |
| Entangled photons in "dark states" | 600x longer than normal (still milliseconds) | 2025 |
| Single trapped ion (one atom, isolated) | Over 10 minutes | 2018 |
| Two entangled ions in a cryogenic trap | ~1-2 hours | Recent |

Clear tradeoff: **the bigger the object, the shorter the entanglement lasts.** Each additional atom adds more ways for the environment to interact with the system and destroy the entanglement. Not that entanglement becomes weaker — the system becomes harder to isolate.

## Why large objects lose entanglement almost instantly

A human body at room temperature:
- Emits and absorbs ~10²³ thermal photons per second per square centimeter
- Is hit by ~10²³ air molecule collisions per second per square centimeter

Each interaction is the environment gaining information about the object's state — effectively "observing" it. Any quantum entanglement between human-scale objects would survive for roughly 10⁻⁴⁰ seconds — a number so small no measurement device could ever capture it.

For comparison, the shortest time ever measured in a lab is about 10⁻²¹ seconds. The entanglement would be gone a billion billion times faster than we could ever detect.

## Entanglement in biology

Despite the hostile environment of warm, wet biological tissue, there's evidence of quantum effects in living systems:

**Photosynthesis:** Plants appear to use quantum coherence (related to entanglement) to transfer energy through multiple pathways simultaneously, achieving near-perfect efficiency. Observed in lab conditions, still debated for living cells.

**Bird navigation:** Some migratory birds sense Earth's magnetic field using a quantum process in molecules in their eyes. Entangled pairs of electrons within these molecules persist for **milliseconds** — longer than entanglement lasts in most laboratory quantum computers. In warm, wet, noisy biological tissue. Biology may have evolved tricks for protecting quantum states that our lab engineering hasn't matched.

**Neurons (very early):** A recent study suggested vibrations in the fatty coating around nerve fibers could generate entangled photon pairs. Not confirmed.

## The open question: correlations beyond quantum entanglement?

Quantum entanglement can't survive at human scales — the math is clear. But this only rules out ONE type of correlation. The question: **are there other forms of correlation between large systems that we don't recognize because we're only looking for the quantum version?**

Bell's theorem proves correlations exist at the quantum scale that exceed what independently-predetermined systems can produce. The question "are there above-threshold correlations at macroscopic scales?" has never been tested — nobody has figured out what a Bell test would look like for two humans or two ecosystems.

We assume the answer is no because the mechanism we know (quantum entanglement) gets destroyed by environmental interaction at large scales. But that's an argument from mechanism: "we don't know a mechanism that could do this, therefore it doesn't happen." History has examples where that reasoning was wrong.

The bird navigation finding is the most suggestive: quantum effects persisting orders of magnitude longer than expected in warm biological tissue. What else biology might be doing that we haven't noticed is genuinely open.

See also: [[photon-entanglement]] [[double-slit-experiment]] [[consciousness-and-the-label-problem]] [[physics-as-perception]]
