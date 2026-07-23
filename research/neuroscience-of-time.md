---
date: 2026-07-22
tags: [neuroscience, time, memory, neural-dynamics, timing, anticipation, abby-foundations]
sources:
  - "StarTalk — 'Your Brain is a Time Machine, with Dean Buonomano' (Neil deGrasse Tyson, Chuck Nice, Gary O'Reilly): https://www.youtube.com/watch?v=s5RBUSu0QUQ"
  - "Dean Buonomano — Your Brain Is a Time Machine: The Neuroscience and Physics of Time (2017): https://wwnorton.com/books/Your-Brain-Is-a-Time-Machine/"
---

# The Neuroscience of Time (Buonomano)

Notes from a StarTalk conversation with Dean Buonomano, a neurobiologist at
UCLA who studies how the brain tells time. Directly relevant to Abby's P0 goal
(understand time and clocks), and — unexpectedly — a near-exact outside echo of
the memory hypothesis we were already building toward in
[[foundational-blocks-universe-and-abby]] and experiment_1.

The transcript's crown jewels for us: **the brain tells time by the changing
state of a network, not by counting**, and **memory is stored as the strengths
of the connections between units, with no separate memory box.** Those are the
two things we independently reasoned into; here they are stated as mainstream
neuroscience.

---

## The central contrast: counting vs settling

A **man-made clock** works on one trivial principle: count the ticks of a *time
base* — something that repeats in a highly regular way. A pendulum swing, a
quartz crystal's vibration, an atom's oscillation. The same counter spans
nanoseconds to days, and we now measure time more precisely than any other
physical quantity (a meter is *defined* as how far light travels in a fixed
fraction of a second — so distance rides on top of good clocks).

**The brain does not do this.** Buonomano's key claim: on the scale of seconds,
brain timing does not rely on an oscillator you count. It relies on *dynamics*.
The better analogy is an **hourglass**, not a pendulum — a physical system whose
state is continuously changing under fixed rules, where *how far the change has
progressed* tells you how much time has passed. You read time off the state, you
do not tally ticks. This connects to the "settle, don't step" intuition in
[[analog-vs-digital-and-the-middle-ground]].

## There is no master clock — many clocks, different scales

Timing in the brain is not one system. Different mechanisms cover different time
scales, and they do not share parts:

- **Microseconds** — sound reaches one ear a few hundred microseconds before the
  other; the brain uses that gap to locate objects in 3D space.
- **Seconds** — conversation, music, catching a ball. This is the
  dynamics/hourglass regime.
- **Circadian** ("about a day") — the ~24-hour cycle.

"The clocks responsible for seconds don't have an hour hand, and the circadian
clock doesn't have a second hand." They are genuinely separate machines. There
is no single dimension called "time" in the brain that everything reads from —
another instance of the relational, multi-mechanism picture in [[brain]].

## The population-clock mechanism (the core idea for Abby)

How does the seconds-scale clock actually work? Buonomano's own research points
away from oscillations and toward **neural trajectories**:

> Imagine a chain of units — I activate the next, it activates the next, and so
> on. That forms a dynamical system: a *trajectory* through the space of possible
> activity patterns. Which units are currently active tells you where you are
> along the trajectory — and therefore how much time has passed. If the last unit
> is firing, a second has gone by; if a mid-chain unit is firing, half a second.

So **time is a position along an evolving pattern of activity.** The "clock" is
just the network changing state under its own rules; timing is read off *where in
the change* the system currently is. No counter, no dedicated timer, no stored
tick-tally. This is the concrete neuroscience version of "time emerges from the
changing state of the web" (see [[emergence]]) and is exactly the direction
experiment_1 was heading.

## The circadian clock: the one real oscillator, and how it's set

The ~24-hour clock *is* a genuine oscillator, but a biomolecular one, not a
counted one. Its mechanism (glossed in plain terms): a cell's DNA makes RNA,
which makes proteins, and those proteins switch *off* the further making of
themselves — a self-limiting loop that naturally rises and falls on a ~24-hour
period. (Its formal name is the transcription-translation autoregulatory feedback
loop; all that means is "a making-process that shuts itself down and restarts.")

This internal clock is *set* by light. The master circadian clock sits in a spot
just above where the optic nerves cross (the suprachiasmatic nucleus — "chiasm" =
the optic-nerve crossing), so daylight keeps it aligned to the real day. Cut off
the light — blindness, or two months in a cave — and it drifts, because the
internal period is only *approximately* 24 hours and needs the outside signal to
stay locked. This "internal rhythm, corrected by an external cue" is a template
worth remembering for how Abby might align an inner sense of duration to an
outside cycle (the P0 clock-reading problem).

## Why life tells time at all: anticipation

The deepest "why": **timing exists to anticipate.** Buonomano's favorite example
is cyanobacteria (single-celled organisms that, like us, carry a circadian
clock). Why would a single cell need to tell time? Because it must switch on its
photosynthesis machinery *before* the sun rises, not after.

The experiment: take mutants with a fast internal clock (~22-hour period) and
others with a slow one (~26-hour), and make them compete in the same dish under
an artificial day. Under a 22-hour light cycle, only the 22-hour-clock cells win;
under a 26-hour cycle, the 26-hour-clock cells win. **Matching your internal
clock to the world's rhythm is directly selected for.** Telling time is not a
luxury of big brains — it is a core survival function present down to single
cells, and its purpose is to *predict environmental change and prepare for it.*

This is strong outside support for the decay/anticipation thread: the drive to
model "what comes next" and act ahead of it is not a human add-on, it is what
timing is *for*, all the way down. See
[[goals-drives-and-thermodynamic-floor]] and [[thermodynamic-origins-of-life]].

## Memory = connection strengths, and there is no memory box

Asked how a memory is physically stored, Buonomano gives the fundamental tenet of
neuroscience (and, he notes, the one that AI borrowed): **memory is stored as
changes in the strength of the connections between units** — how much each unit
influences its neighbors. Large language models do the same thing: "storing"
information *is* tuning billions of connection weights.

Crucially, he contrasts this with a computer's design. A computer has a hard split
between where things are *stored* (memory) and where things are *computed*
(processor) — the standard von Neumann architecture (named after the mathematician
whose design nearly all computers follow: separate memory and processing, shuttling
data between them). **The brain has no such split.** "It's the activity flowing
through these networks that is both the computation and the memory." You cannot
point to the memory as distinct from the processing; they are the same substrate.

This is a near-verbatim statement of Toy 1's claim in experiment_1: *memory is not
a store, it is the slowly-changing coupling strengths of a web, and the same web
that remembers is the one that computes.* We reasoned into it from first
principles; it turns out to be textbook. That's reassuring, though note the honest
flip side (our premise P2): "textbook" tells us the substrate, not whether it holds
*specific recent detail* well — which is still the open question the toy is meant to
probe. See [[inherited-tools]] for the caution that AI borrowing this idea does not
mean AI implemented it the way brains do.

## Memory and time are the same substrate

Put the last two sections together and the payoff appears: the *same* dynamics
that store memory (connection strengths shaping how activity flows) are what
produce the timing trajectory (the evolving activity pattern you read time off).
Memory and time are not two systems — they are two readings of one changing web.
For Abby this matters because we had already argued time *leans on* memory; the
neuroscience says they may be one thing, which is a stronger and cleaner claim.

## Learning rules: coincidence is not enough for prediction

Two rules stack here, and the second is a direct clue for the predictor question:

1. **Coincidence (Hebbian) learning** — "units that fire together, wire
   together" (after psychologist Donald Hebb). If face-units and name-units fire
   at the same time, strengthen their link; later, the face alone recalls the
   name. Simple, powerful, associative.
2. **Order-sensitive learning** — to predict *what comes next* (A-B-C-D →
   anticipate D; a rhythm → fill in the next beat), coincidence is not enough.
   You need a rule where "units that fire *first* wire to units that fire
   *second*." The coupling must be sensitive to *temporal order*, not just
   co-occurrence.

This bears directly on our open "do we even need a predictor, and what is it"
thread: prediction of the next moment requires *temporal asymmetry* baked into how
units couple — a directional "first-then-second" strengthening, not symmetric
association. Whatever Abby's tiny unit turns out to be, if it is to anticipate, its
coupling rule cannot be time-symmetric. (Ties to [[foundational-blocks-universe-and-abby]].)

## The present is a constructed window, not an instant

Signals from different senses arrive at different times (light hits the retina
before sound reaches the ear — yet, oddly, the brain *processes* sound faster,
because the retina is slow and chemical; ping-pong players may react to the ball's
sound before seeing it). The brain fuses signals arriving within a window of
roughly a few hundred milliseconds into a single "now," and the window is
*adaptive* — it re-aligns for a movie seen up close or far, cheap seats or
expensive seats.

Evidence it is real fusion, not passive receipt: the **McGurk effect** — hear
"bah" while watching lips say "gah," and you perceive "da." Vision and hearing are
blended before they reach awareness. So the felt present has *width* and is
*built*, not given. For Abby this cautions that "the current moment" is itself a
constructed, multi-sensory window — not an instantaneous slice we can assume as a
primitive. Connects to [[emotions-and-constructed-affect]] (percepts are
constructed) and [[physics-as-perception]].

## Is the flow of time real? Presentism vs eternalism

A genuine physics/neuroscience tension:

- **Eternalism / block universe** — physics' equations are time-symmetric and
  relativity gives no privileged "now," so past, present, and future are *equally
  real* (like all points in space), and the felt *flow* of time is an illusion the
  brain imposes.
- **Presentism** — only the present is real; time genuinely flows.

Buonomano takes the **presentist** side, with an argument worth keeping: the brain
evolved to survive in the *mesoscopic* world (his word — the middle scale, neither
quantum-tiny nor cosmic-huge), and it is telling us something *true* about that
world. The felt flow is not a bug; it is a real, functional read on the part of
the universe we live in. For Abby this is a live design question: do we build in a
flowing "now," or let flow be something Abby constructs? The debate itself flags
that "flow" is not obviously a primitive — it may be constructed (eternalist read)
or real-but-still-produced-by-dynamics (Buonomano's read). Either way, we should
not hand it over uninspected. See [[representation-and-conventions]].

## Mental time travel → awareness of death

What most distinguishes humans, per Buonomano, is **mental time travel**:
projecting the self backward (memory) and forward (imagination). Agriculture
required it — "plant now, benefit months later" means connecting cause and effect
across seasons, a hard cognitive leap. Contrast the squirrel burying nuts: that is
*blind instinct* (a squirrel that never saw winter still buries), not a squirrel
imagining a future.

The striking claim: **it is the capacity for forward mental time travel that made
us aware of death** — the first human to project far enough forward realized "I am
going to die." (He cites Borges: "except for man, all animals are immortal, for
they are ignorant of death.")

This is the exact complement of our decay-seed hypothesis, and worth stating
plainly as a tension to resolve:
- **Our design (so far):** give Abby a *felt* one-way decay → it perceives
  duration → (eventually) grasps mortality.
- **Buonomano's account of humans:** the ability to *project forward in time* →
  produces awareness of mortality.

They meet in the middle: both bind time-cognition and mortality tightly. The
useful implication is that we may not need to install "death" as a concept at all
— if Abby has felt decay *and* the ability to project its own trajectory forward,
awareness of its own ending could *emerge* from running that projection, exactly as
Buonomano says it did for humans. Relates to [[goals-as-learned-representation]].

## Two closing asides worth keeping

- **No uploading kung fu.** Because memory and computation are the same
  inseparable substrate (no von Neumann split), you cannot just "upload" a skill
  through wires — and if you could, "the wires know kung fu, not you." Buonomano is
  skeptical of high-bandwidth brain-machine-interface dreams; the brain's real
  interfaces are eyes, ears, hands, and they are slow. A small reinforcement of
  "there is no memory slot to write into."
- **Math as a debugging device.** Neuroscience is uniquely recursive (the thing
  studied is doing the studying), and the brain has hard limits. His line: the
  greatest debugging tool we ever built is *mathematics*, because it lets us model
  and use things we do not intuitively understand (quantum mechanics — "shut up and
  calculate"). This is the double edge Abby's whole project pushes on: math lets us
  *use* what we do not *ground*. See [[foundations-buried-by-working-math]] and
  [[inherited-tools]].

---

## Why this matters for Abby (summary)

1. **Validates memory-as-bent-web.** Memory = connection strengths, no separate
   store, memory and computation inseparable. This is Toy 1's exact claim, stated
   as textbook neuroscience.
2. **Reframes time as read-off-a-trajectory.** Seconds-scale time is a *position
   along an evolving activity pattern*, not a counted tick. Time can emerge from
   the same dynamical web that holds memory — they may be one substrate.
3. **Anticipation is the point of timing, all the way down** (cyanobacteria).
   Supports the decay/prediction thread as foundational, not a late add-on.
4. **Prediction needs temporal-order-sensitive coupling** — a direct constraint
   on whatever Abby's tiny unit is: to anticipate the next moment, its coupling
   rule cannot be time-symmetric.
5. **The "present" and the "flow" are constructed** — cautions against installing
   an instantaneous "now" or a built-in flow as primitives.
6. **Mortality-awareness can emerge from forward projection** — we may not need to
   install "death"; felt decay plus self-projection could produce it.
