---
date: 2026-06-30
tags: [fundamental-physics, ontology, structural-realism, information-physics, substrate, abby-foundations]
sources:
  - https://en.wikipedia.org/wiki/Quantum_field_theory
  - https://arxiv.org/html/physics/0107050v13
  - https://en.wikipedia.org/wiki/Quantum_entanglement
  - https://jdlongmire.github.io/logic-realism-theory/topics/wheeler/
  - https://arxiv.org/pdf/1303.6007
  - https://durham-repository.worktribe.com/output/1638590/relations-all-the-way-down-against-ontic-structural-realism
  - https://en.wikipedia.org/wiki/Constructor_theory
  - https://www.quantamagazine.org/with-constructor-theory-chiara-marletto-invokes-the-impossible-20210429/
  - https://activeinference.github.io/papers/process_theory.pdf
---

# Foundational Blocks: the Universe, and what Abby should start from

The question that started this note: *what is the foundational block of the
universe — should we build Abby up from electrons / protons / atoms? What is a
sound thing to start with?*

Short answer up front: **modern physics stopped bottoming out in little hard
balls a century ago, and even if it hadn't, "what the universe is made of" is the
wrong question to copy for Abby.** Those are two different questions, and the most
useful result of this research is keeping them apart.

## Part 1 — What does physics actually treat as fundamental?

A walk down the ladder, each rung dissolving the one below it as "the bottom":

### Atoms and particles are *not* the floor

The atomist intuition — reality is tiny indivisible balls, stack them up to get
everything — is intuitive and, as fundamental physics, wrong. Atoms are made of
protons, neutrons, electrons; protons and neutrons are made of quarks. And the
deeper you go, the less ball-like it gets.

### Fields are deeper than particles

In **quantum field theory** (our best-tested framework), the truly basic objects
are **fields** — quantities that have a value at every point in space, filling
everything. A "particle" is a *ripple* in a field: an electron is a quantized
vibration of the electron field, a photon a ripple in the electromagnetic field.
So the electron is not a thing, it is *an excitation of a thing that is
everywhere.* Particles are behaviors of fields, not bricks.

### Maybe even space and time are not fundamental

The frontier goes further. A major line in quantum gravity (holography, the
AdS/CFT correspondence, "spacetime from entanglement," ER=EPR) suggests
**spacetime itself emerges** from the entanglement of more basic degrees of
freedom — that the geometry connecting two regions is a picture of how much their
quantum information is shared. If that holds, space and distance are not the
stage; they are *output.* See [[entanglement-scale-and-boundaries]],
[[bell-theorem-and-nonlocality]], and [[vacuum-and-entropy]].

### Three candidates for "the actual bottom"

Since particles, and maybe spacetime, are emergent, what is left? Three serious
proposals, all of which matter for Abby:

1. **Information** ("it from bit", Wheeler): every physical thing derives from
   yes/no answers — bits. Reality is information-theoretic at root; the universe
   is more like an answer to questions than a box of stuff. See
   [[information_processing]].
2. **Relations / structure** (ontic structural realism): there are no
   fundamental *things* with relations laid on top — there is only **relational
   structure**, and "objects" are just stable knots in it. The most radical
   version is literally "relations all the way down," with no relata (no things
   being related). This is contested (critics ask how you can have a relation
   with nothing being related), but it is taken seriously.
3. **Tasks / what is possible** (constructor theory, Deutsch & Marletto): stop
   describing the world as "state now → state later under equations" and instead
   state which **transformations are possible vs impossible, and why**. A
   "constructor" is anything that can perform a task repeatedly without being
   used up (a catalyst, a machine, a living cell). This reframes physics around
   *capabilities* rather than *substances*, and is explicitly built to cover the
   physics of life and of information — the things substance-physics handles
   badly.

The thread through all three: **the deepest layer is not stuff, it is pattern —
relationships, information, and what-can-be-done.** This is the physics-side echo
of the epistemology in [[representation-and-conventions]] (we capture structure,
not intrinsic nature) and connects to [[emergence]] (complex behavior from simple
relational rules) and [[analog-vs-digital-and-the-middle-ground]] (is the bottom
layer discrete bits or a continuous medium?).

## Part 2 — Why this does NOT mean "build Abby from electrons"

Here is the trap, stated plainly: **the universe's foundational block and Abby's
foundational block are different questions, and treating them as the same is a
category error.**

Reasons to *not* start Abby at electrons/atoms/physics-from-scratch:

- **The universe itself doesn't build understanding from electrons.** Learning,
  meaning, prediction — none of these live at the electron level. They are
  high-level *relational* phenomena. Simulating quarks would rebuild a
  *substrate*, not a *learner*. You would spend everything modelling the stage
  and never reach the play.
- **It is the wrong altitude and intractable.** Even the best supercomputers
  cannot simulate a single bacterium atom-by-atom in real time. Building a baby
  mind on simulated protons is not a slow path, it is a closed one. See
  [[energy-cost-of-intelligence]].
- **It re-imports the atomist mistake we just saw physics abandon** — that you
  reach the interesting thing by stacking tiny bricks. Even physics found that
  the interesting structure is relational and emergent, not assembled.

So the right move is to choose Abby's primitive at **the altitude where learning
actually lives**, and let lower levels be whatever cheap substrate carries it.

### What level *does* learning live at?

From [[representation-and-conventions]] and experiment_1: the smallest thing that
can *learn* is the smallest thing that can **hold a guess, meet reality, and
change because it was wrong.** Not a symbol, not a static value, not a particle —
a **tiny self-correcting predictor.** That is Abby's electron: the irreducible
unit at the learning altitude. Representation is then the *relationships between
predictors* — which is exactly the relational/structural ontology physics landed
on, applied one level up. We are not copying the universe's bricks; we are copying
the universe's *style* (relations and prediction over substance).

### Candidate substrates (the layer *under* the predictor)

If the predictor is the brick, what carries it? This is the real "what to build
on" decision, and it maps onto the A/B fork in experiment_1:

- **Discrete / digital** — predictors as small programs/networks updated in
  steps. Easy to build, but bakes in a clock and a symbol grain we may not want.
- **Continuous / analog** — predictors as a physical or simulated continuous
  medium that settles into agreement (dynamical systems, analog computing,
  neuromorphic hardware, reservoir computing). Closer to "fields settling," lets
  structure emerge instead of being coded. See [[analog_computing]] and
  [[analog-vs-digital-and-the-middle-ground]].
- **Possibility-first (constructor-theory flavored)** — define Abby by which
  transformations its predictors *can and cannot* perform, rather than by a state
  update rule. Speculative, but it is the framing that natively handles
  information and life, which is what Abby is.

Two outside frameworks already build agents at roughly the predictor altitude and
are worth mining for the substrate decision:

- **The free-energy principle / active inference** (Friston): an agent is a thing
  that keeps itself in its expected states by minimizing the gap between its
  predictions and its sensations — *and* acts to make the world match its
  predictions. This is Engine 1 written as physics, and it comes with math for
  how such an agent persists. See [[goals-drives-and-thermodynamic-floor]] and
  [[thermodynamic-origins-of-life]].
- **Cellular-automata / emergence view**: complex structure from many copies of a
  simple local rule. The relational-physics result says the bottom is simple
  relations producing emergent complexity; a learner could be built the same way
  — many tiny predictors, local interactions, structure emerging. See
  [[emergence]].

## Bottom line for Abby

- Do **not** start from electrons/atoms/simulated physics. Physics itself shows
  the foundation is not tiny bricks but **relations, information, and
  possibility**, and understanding does not live at the particle altitude
  anyway.
- Start at the **learning altitude**: the foundational block is a *tiny
  self-correcting predictor*, and representation is the *relationships between
  predictors.* This copies the universe's relational *style*, not its bricks.
- The genuinely open decision is the **substrate under the predictor** — discrete,
  continuous/analog, or possibility-first. This is the experiment_1 A/B fork, and
  the physics result mildly favors a relational/continuous substrate where
  structure can emerge rather than be hand-assembled.

## Open threads

- Is the bottom layer of *reality* discrete (bits) or continuous (fields)? The
  field view says continuous; "it from bit" says discrete. Abby's substrate
  choice secretly rides on which intuition we trust. See
  [[analog-vs-digital-and-the-middle-ground]].
- If spacetime is emergent from relationships, should Abby even have a built-in
  clock/space, or should time and space emerge from the predictors' relations
  too? (experiment_1 currently builds time in — this questions that.)
- Constructor theory says describe a thing by what it *can do*, not its states.
  Is "what transformations can this predictor reliably perform" a better handle
  on a learner than "what does it output"?
