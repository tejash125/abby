---
date: 2026-05-02
tags: [physics, quantum, observation, wave-particle, foundational]
sources:
  - "Young, Thomas — On the Theory of Light and Colours (1801)"
  - "Jönsson, Claus — electron double slit (1961)"
  - "Kim, Yoon-Ho et al. — Delayed Choice Quantum Eraser (2000)"
  - "Arndt et al. — large molecule interference, University of Vienna"
  - "youtube: The Weird Experiment that Changes When Observed (5kfGRO6msQw)"
  - "youtube: The Original Double Slit Experiment (Iuv6hY6zsd0)"
  - "youtube: Double Slit Experiment explained by Jim Al-Khalili (A9tKncAdlHQ)"
---

# Double Slit Experiment

## Setup

A wall with two narrow vertical slits. Behind it, a screen that records where things land.

**Sand grains** through the slits → two piles behind the two slits. Particles behave like particles.

**Water waves** through the slits → wave passes through both slits simultaneously. Two new waves spread from each slit and interact. Where peaks meet peaks, they add up (bright band). Where peaks meet valleys, they cancel (dark band). Result: a striped pattern of alternating strong and weak bands. This is an interference pattern — what happens when two waves combine.

## The strange result

Shoot electrons (or photons) one at a time. Each one is a single particle — it lands as a single dot at a specific spot on the screen. You'd expect two piles, like sand.

Instead, as dots accumulate, they form the wave interference pattern. Many bands, not two piles. Each individual particle lands as a definite dot, but the *distribution* of where those dots land follows the pattern you'd only expect from waves passing through both slits and interfering.

One particle. Apparently going through both slits. Interfering with itself. Landing as a single dot.

This is not a statistics trick. Slow it down to one particle per hour. Same result.

## The observer effect

Place a detector at the slits to record which slit each particle goes through. Just recording, not blocking.

The interference pattern disappears. Two piles, like sand. Particle behavior.

Remove the detector → interference comes back. Wave behavior.

### What "observation" means here

"Observer" does NOT mean a human looking at it. It means any physical interaction that extracts information about which path the particle took. The detector must interact with the particle to detect it — typically by bouncing a photon off it. That physical interaction is the "observation."

The natural objection: **isn't the detector just physically kicking the particle?** Of course the pattern changes — you're disturbing it. This is a valid objection for the basic version of the experiment.

## The entangled photon version (quantum eraser)

A more sophisticated experiment was designed specifically to test whether it's just physical disturbance:

1. Create entangled photon pairs (see [[photon-entanglement]]). Two photons born from one event — photon A and photon B.
2. Send photon A toward the double slits. No detector at the slits. Nothing touches A.
3. Send photon B to a separate detector far away.
4. Because A and B are entangled, measuring B can reveal which slit A went through — without ever touching A.
5. When B's measurement reveals which-path information → no interference pattern for A.
6. When B's detector is set up to destroy the which-path information → interference pattern for A comes back.

Nobody kicked photon A. The only thing that changed was whether information about its path existed anywhere.

### The critical catch

Looking at ALL the dots photon A makes on the screen — without knowing anything about photon B — you see no interference pattern. Just a featureless blob. Always. Regardless of what was done to B.

The interference pattern only becomes visible when you **sort** A's data based on what B's detector recorded:
- Filter for A dots whose partner B was measured in the information-erasing way → that subset shows interference
- Filter for A dots whose partner B was measured in the information-preserving way → that subset shows no interference

Both subsets hit the same screen at the same time. Mixed together, they cancel into a blur. The pattern is hidden in the correlations between A and B, not in A alone.

This means:
- Measuring B does NOT send a signal to A that rearranges where A lands. Individual landing spots don't change.
- But the correlations between A and B do depend on how B was measured.
- The physical-kick explanation doesn't work (nobody touched A).
- The "consciousness causes collapse" interpretation doesn't work either (the overall pattern on A's screen never changes).

## Scale limits

| What was tested | Size | When |
|---|---|---|
| Photons (light) | No mass | 1801 (Thomas Young) |
| Electrons | Extremely tiny | 1961 |
| Individual atoms | Single atom | 1990s |
| Molecules of 60 carbon atoms | 720 atomic mass units | 1999 |
| Molecules of ~810 atoms | 10,000 atomic mass units | 2013 |
| Molecules of ~2,000 atoms | 25,000 atomic mass units | 2019 |
| Sodium clusters (5,000-10,000 atoms) | 170,000+ atomic mass units | 2025 |

The reason it doesn't work for large objects like a tennis ball isn't a hard mass limit — it's about interaction with the environment. A tennis ball at room temperature is constantly being hit by trillions of air molecules and photons every second. Each interaction effectively "detects" the ball's position. The wave-like behavior gets destroyed almost instantly because the environment is constantly gaining information about where the ball is.

The tiny particles in experiments work because they're isolated — in a vacuum, cooled to near absolute zero, shielded from stray light. The experimenters go to extreme lengths to prevent the environment from "detecting" the particle before it reaches the screen.

Nobody has found a hard mass limit where the physics changes. It just gets exponentially harder to keep larger things isolated from their environment.

## What's established vs what's open

**Established:**
- Single particles produce interference patterns (wave-like behavior)
- Gaining which-path information destroys the pattern (particle-like behavior)
- This isn't just physical disturbance — the entangled photon experiments rule that out
- The effect scales up to molecules of thousands of atoms when properly isolated
- No hard mass limit has been found

**Open:**
- What is the particle "doing" between emission and detection? Does it go through both slits? Does the question even make sense?
- Why does the availability of which-path information matter? What does "information" mean physically?
- "Particle" and "wave" are labels from everyday experience. The electron is neither — it's something our language doesn't have a word for because we never evolved to experience it

See also: [[photon-entanglement]] [[vacuum-and-entropy]] [[consciousness-and-the-label-problem]] [[physics-as-perception]]
