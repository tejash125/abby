# Toy 1 — Memory as a slow-bending web (idea file)

Status: **idea file, pre-code.** Per project convention, this English description
exists before any code is written, and code is derived from it. Originally framed
around a "web of tiny predictors"; reframed after pressure-testing what a predictor
smuggles in (see "Why compression, not prediction" below). The memory-as-bent-web
spine is unchanged; what changed is *how structure gets into the web.*

## The claim this toy tests (two parts)

1. **Memory is not a store. It is the slowly-changing strengths of the couplings in
   a web.** No buffer, no slot, no saved copy of the past — a system can still hold a
   pattern purely because its connections got bent by having seen it. If true, Abby
   has no "memory box"; the past lives in the current shape of the web.
2. **Structure gets into those couplings by compression under scarcity, not by
   predicting the next moment.** A web with too few resources to hold a pattern
   verbatim is *forced* to capture the pattern's structure and represent it with
   little — and it can then regenerate the pattern, or complete it from a partial cue.

If part 1 fails, Abby needs a fast explicit trace after all. If part 2 is the wrong
cut, we learn that structure-capture needs something more than scarcity.

## Why compression, not prediction (the key move)

The earlier version made each unit *guess its own next value.* Pressure-testing that
surfaced a problem: "guess the **next** value" bakes the **arrow of time** into the
primitive — and installing time as a given is exactly what this project keeps trying
*not* to do.

The deeper fact that dissolves the choice: **prediction and compression are the same
underlying achievement — capturing regularity — seen from two angles.** To compress,
you find what repeats and store only the *surprises* (the parts you couldn't have
guessed). But "the part you couldn't have guessed" is exactly what a predictor fails
to predict. A perfect predictor gives perfect compression; any good compressor
secretly contains a predictor. They are two outfits on one capability.

So the real question is *which outfit to build first*, and that choice decides what
we smuggle in:

- **Prediction faces *time*** — "complete the *next* moment" — and bakes in the arrow
  of time.
- **Compression / retrieval faces *structure*** — "find what repeats in *what is*,
  store it small, get it back from a part" — and bakes in **nothing about time.** It
  can run on a single static snapshot.

We build the structure-facing outfit first because it assumes less. Prediction is not
discarded — it becomes an **emergent use** we watch for *later*, once the time axis is
added for P0. Completing a pattern in *space* (fill the missing part) and predicting
it in *time* (fill the next moment) are the same operation — **pattern completion** —
aimed at different axes. This toy points it at the axis that assumes less.

(Note: memory-as-compression-into-couplings, and the hint that memory and time may be
*one* substrate, are exactly what the neuroscience says — see
`research/neuroscience-of-time.md`.)

## Don't install a predictor — or a compressor. Install scarcity.

The strongest form of the reframe: install **neither** capability. Install a
**condition** and let the capability grow, in the project's usual style.

- Install **scarcity** — few internal units, or a tight resource/energy budget (the
  decay-seed's close cousin; a finite budget is literally what forces pruning and
  efficiency in biology, see `research/mitochondria-and-energy.md`).
- Feed that scarce web a **patterned world.**
- Now the web *cannot* hold the pattern verbatim — no room — so the only way to hold
  it at all is to **capture its structure and represent it with little.** Compression
  is *forced by scarcity*, not coded as a mechanism.
- Once structure is captured, **retrieval** (complete from a cue) and, later,
  **prediction** (complete the next) both fall out as *uses* of it.

This quietly unifies three things we had kept separate: the **decay seed** (scarcity),
**memory-as-bent-web** (the captured structure lives in the couplings), and
**prediction** (a later use). One story.

## The four premises this sits on (holes to keep in view)

From the office-hours session:

- **P1 (dark room):** a surprise-minimizing system can cheat by hiding where nothing
  happens. Not tested here (no action, no survival) — do not let it creep in.
- **P2 (memory-detail gap):** the no-store idea may cover blurred averages but fail on
  *specific* detail. This is now sharpened into the **lossy-vs-lossless** question:
  does the compact code keep specific detail, or smear everything into a useless
  average? **This toy is the direct test of P2.**
- **P3 (continuous→discrete):** the continuous substrate is right, but the jump to
  discrete symbols is its own hard problem. Not tested here.
- **P4 (isolate):** test one claim cleanly. This toy obeys P4.

## What the toy is

**World:** a repeating pattern in a continuous signal. Crucially it can be **static** —
a spatial shape — so **no time is needed.** (A short repeating sequence is allowed,
but we do *not* lean on its "next-ness.")

**Agent:** a **scarce** web — deliberately too few active units, or too tight a budget,
to store the input verbatim. It forms a compact internal state from the input and can
**regenerate** the input, or **complete** it from a partial cue, out of that compact
state. Memory lives in the couplings. There is deliberately **nothing** named
"memory," no store, no delay line — and now, nothing named "predictor," no "next."

**Grading (self):** *reconstruction / retrieval error* — did what it regenerated match
the input? This is self-supervised, needs no teacher, and keeps the self-grading
property we cared about in Engine 1 (the world/its-own-reconstruction tells it when
it's wrong).

**The test:**
1. Give a **partial cue** — does the web complete the rest? (retrieval)
2. How **compact** can the internal code get before reconstruction breaks?
   (compression)

## Success and failure (measurable, decided up front)

- **Success:** from a partial cue, or after being squeezed through the scarce
  bottleneck, the web regenerates the pattern below an error threshold. Structure is
  living in the couplings, captured compactly, with no store.
- **Failure:** it can only reproduce what it is *currently being shown* — partial or
  remove the input and it collapses to noise or a flat line; **or** it "compresses"
  only by blurring everything into a useless average. Either means the no-store idea
  fails for the detail we need, and Abby needs a fast explicit trace (P2 confirmed).
  A *useful* failure — it resolves a real open question.

Guardrails so the result is honest:
- No explicit buffers or delay lines anywhere.
- The knobs under study are **(a) how scarce** (how narrow the bottleneck / how tight
  the budget) and **(b) how slowly the couplings change** — too fast forgets, too slow
  never learns.
- No decay-as-drive, no action, no reward, **no arrow of time** in this toy — those
  belong to later claims.

## Honest costs we are choosing to defer

- **Retrieval hides an addressing problem** — "which stored thing matches this cue"
  assumes the web knows *where* its stuff is. Biology uses a dedicated indexer (the
  hippocampus, see `research/brain.md`). We hand-wire addressing for now — a **scaffold
  to remove later**, like the clock we refused to build in.
- **Lossy compression needs a notion of "what matters"** = relevance = stakes = decay.
  We sidestep it: start lossless-ish, or let the *scarcity itself* decide what drops.
  We do **not** hand-code importance.
- **Time is deferred.** P0 (clocks, time, drawing) is fundamentally time-facing, so
  prediction-of-the-next must return *later* as an emergent use. This toy isolates
  structure-capture on purpose — it is the honest *starting* move, not a permanent
  escape from time.
- **The scarcity level and the wiring are still our choices** — the same "we chose the
  structure" scaffold as before, just relocated from "what predicts what" to "how
  scarce, how wired." Name it; plan to remove it.

## Substrate note (A/B fork deferred, not decided)

This toy does not resolve the discrete-vs-continuous substrate fork. To build the
smallest honest version we will simulate continuous-valued units in discrete steps —
chosen for convenience, **not** as a commitment. The fork stays open. (Computational
irreducibility says we cannot derive the web's behavior from the armchair anyway — we
have to run it; see `research/computational-irreducibility.md`.)

## Approaches considered (from office hours)

- **A — Time from decay:** most direct to P0, but time leans on memory, so it risks
  failing for memory reasons. Deferred.
- **B — Memory as slow web (this one):** the foundational claim everything depends on.
  **Chosen** — proving/breaking it first de-risks the rest.
- **C — Life, not a rock:** tests the survival drive / dark-room escape. Important, but
  tests the drive, not memory. Deferred.

## Not in scope

No arrow of time / prediction-of-the-next (emergent later), no decay-as-drive, no
goals, no action, no second agent, no conventions, no discrete symbols. This toy is
**structure-capture under scarcity, alone.**
