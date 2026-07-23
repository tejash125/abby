---
date: 2026-07-22
tags: [computation, complexity, emergence, evolution, machine-learning, irreducibility, abby-foundations]
sources:
  - "Stephen Wolfram — 'The universe isn't random – it's something stranger' (The Well / Big Think): https://www.youtube.com/watch?v=U8Omt6K8OnM"
  - "Wolfram, A New Kind of Science (2002); Wolfram Physics Project"
---

# Computational Irreducibility

We touched this idea before ([[emergence]], [[digital_computing]]); this note goes
deeper, from a short Stephen Wolfram talk. It matters for Abby more than it first
looks, because it is the *formal reason* we cannot reason our way to Abby's design
from the armchair — and the formal reason a learner that actually works will be one
we cannot fully explain. Both of those cut straight across the project's ethos, so
they are worth stating carefully.

## The core idea, in plain terms

Take a simple program with fixed, deterministic rules. You want to know what it will
be doing after a million steps. There are two possibilities:

- **Reducible** — you can *jump ahead*. There is a shortcut, a formula, that tells
  you the state at step one million without going through the steps. This is the
  dream of the exact sciences: you do not simulate a million orbits of the Earth to
  know where it will be; you use a formula and leap to the answer.
- **Irreducible** — there is *no shortcut*. The only way to find out what the
  program does at step one million is to actually run all one million steps and
  watch. Knowing the rules perfectly does *not* let you predict the behavior; you
  still have to run it.

**Computational irreducibility** is the claim that most interesting computational
systems are of the second kind. There is an *irreducible gap* between the underlying
deterministic rules and the actual behavior — even though the behavior is fully
determined by the rules, the only way to know it is to let it play out. This is
different from randomness (the system is not random — it is exactly determined) and
different from chaos (it is not about sensitivity to initial conditions). It is
about the *absence of a computational shortcut*.

## Where it comes from: simple rules, complex behavior

Wolfram's foundational finding (the spine of *A New Kind of Science*): in the space
of all possible simple programs, **even a very simple program can produce extremely
complicated behavior.** You do not need complicated rules to get complicated
results. He argues this is the secret nature uses to make its complexity — the
spiral growth of a mollusk shell, the pigmentation patterns on it — a simple
underlying rule, run, producing elaborate structure. This is the engine under
[[emergence]] and the reason Abby's whole bet (many tiny units + simple local rules
→ structure emerges) is even plausible.

## Evolution ≈ machine learning, and why this frames Abby's design

Wolfram's recent move: biology was never a theoretical science — Darwin expected
some abstract law governing evolution's progress, and none was found. Why doesn't
evolution get *stuck*? Why can it keep producing more elaborate forms? His answer
came from noticing that **machine learning works the same way**. (Machine learning:
take a network of simple tunable units — a "neural net" — and adjust it against
examples over and over until it does something useful. Wolfram had failed to make
neural nets do anything interesting in the 1980s; the 2010s surprise was that if you
just "bash it really, really hard," eventually it learns.)

The mechanism he sees in both:

> Building a wall by *engineering* means making regular bricks and stacking them in
> a simple pattern. Building it the way biology and machine learning do means picking
> up **random lumps of irreducible computation** — like rocks lying on the ground —
> and finding that *this* one happens to fit *here*, and gradually assembling a wall
> out of found, pre-computed pieces.

And the crucial condition for why this *works*:

> Evolution works because the **fitness objectives are computationally simple
> compared to the power of the underlying irreducible computation.** If every
> organism had to solve an elaborate math problem the moment it was born, none would
> survive. Because the survival bar is *computationally cheap* relative to the rich
> computation available in the substrate, evolution can keep finding pieces that
> clear the bar.

This maps almost exactly onto Abby's architecture, and reframes it usefully:

- The **substrate** (a web of many tiny units) is the source of *powerful
  irreducible computation* — the "rocks lying around."
- The **decay seed / survival pressure** ("don't hit zero") is a *computationally
  simple fitness objective*.
- The bet is that a simple pressure over a rich, irreducible substrate is exactly
  the regime where complexity (goals, memory, time, concepts) can *emerge* rather
  than be hand-built.

That is not a loose analogy — it is the same structural claim Wolfram makes for why
biology and ML work at all. It is the strongest outside case yet that our "simple
built-in pressure + rich substrate, let the rest emerge" plan is a real mechanism,
not wishful thinking. See [[foundational-blocks-universe-and-abby]] and
[[goals-drives-and-thermodynamic-floor]].

## The hard consequence for Abby: you have to run it

Here is the part that bites. If Abby is a genuinely powerful computational learner,
it will be **computationally irreducible.** That means:

1. **We cannot shortcut it from the armchair.** There is no formula that tells us
   what the web will do without running the web. This is the formal backing for a
   thing already said in the predictor discussion — "we can't reason our way to the
   predictor's true form; the experiments are how we find out." Computational
   irreducibility says that is not a temporary lack of cleverness; it is a wall. The
   toys are not a convenience, they are the *only* instrument.
2. **A working Abby will not be fully explainable.** It "can always surprise us... do
   things where you can tell what it does only by following the steps and seeing." A
   powerful learner is, by this argument, necessarily one whose behavior we can watch
   but not derive.

This sits in real tension with the project's core rule ("explain everything from
first principles; if it can't be explained to a kid, we don't understand it well
enough"). Computational irreducibility says: for the *rules* — yes, keep those
simple and fully understood. For the *behavior* they produce — no, you may never get
to explain that by shortcut; you will only get to run it and observe. The honest
reconciliation is probably: **we owe first-principles clarity about Abby's rules and
seeds, and we accept irreducibility in Abby's grown behavior.** Worth holding this
tension openly rather than pretending we will "understand" a working Abby the way we
understand a formula. Connects to [[foundations-buried-by-working-math]] and
[[inherited-tools]] (the recurring warning about using what we cannot ground).

## The wider framing: use-without-understanding, and AIs as an alien civilization

Wolfram sets computational systems against the Industrial Revolution. Post-industrial
machines (gears, levers) we *understood* — reducible by design. But before that, we
used things we did not understand: you ride a horse, you know what it can do, you
have no idea how it works inside. Computational machines return us to that
pre-industrial condition — *use without understanding* — and it is a genuine societal
choice: insist a machine be reducible (understandable but sharply *limited* in what
it can do) or allow it to be irreducible (able to use its computation fully, but
capable of surprising us and never provably safe).

He extends this: the AIs are becoming "an alien civilization right in front of us."
But we already live beside one — **nature** — which also computes endlessly, and
which we have learned to coexist with (we build houses so the rain does not bother
us) without controlling or fully understanding it. A useful mental model for how one
might live alongside irreducible systems, Abby included.

## A last thread: mortality and never being "done"

Two asides worth keeping. First, Wolfram thinks *humans* remain special not despite
but *because of* the whole bundle — including **mortality** and particular sensory
experience — which AIs lack. That rhymes with the decay-seed and with Buonomano's
"mental time travel made us aware of death" in [[neuroscience-of-time]]: finitude
keeps showing up as central to what a mind *is*, not incidental to it. Second:
technology is "taking what exists in nature and applying it to human purposes," and
computational irreducibility guarantees there is *always more to find* — so we are
never done. The drive to keep seeking the new he reads as a vestige of three billion
years of natural selection. Again: an open-ended pressure, not a fixed goal.

---

## Why this matters for Abby (summary)

1. **The mechanism under the whole bet.** Simple rules can produce unbounded
   complexity; that is why "tiny units + simple local rules → emergent structure" is
   a real mechanism, not hope.
2. **Simple objective + rich substrate is *the* regime that works** — Wolfram's
   explanation for evolution and ML is the exact shape of Abby's design (decay
   pressure over a web).
3. **We must build and run — there is no shortcut.** Computational irreducibility is
   the formal reason the toys are the only way to learn Abby's answers; armchair
   derivation is ruled out, not just hard.
4. **A working Abby will be explainable in its *rules* but not in its *behavior*** —
   a real tension with the project's first-principles ethos, to be held honestly:
   clarity about seeds, acceptance of irreducibility in what grows.
5. **Mortality keeps recurring as central to mind** — reinforcing the decay-seed
   from yet another direction.
