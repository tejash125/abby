# Abby — Artificial Baby

A long-term, **highly opinionated** research project trying to understand intelligence from the ground up — and through it, the physical world and the foundations underneath both — by rebuilding from first principles instead of stacking on top of what already exists.

> **Read this first.** This is opinionated research, not a textbook and not a balanced survey. It takes positions, states them plainly, and tries to be honest about where they could be wrong. It is a public thinking log: half-formed ideas, dead ends, and strong claims all kept in the open on purpose. If you want settled consensus, this is the wrong repo. If you want to argue about foundations, welcome.

## The question

The long-term aim is bigger than building an artificial baby. It is to challenge accepted ideas and rebuild understanding from first principles: the physical world, intelligence, and the foundational blocks of the universe — and eventually the questions underneath all of it, *who are we and what are we doing here.*

**Intelligence comes first** — not because it is separate from the rest, but because it is the thing doing the asking. Whatever lets a mind even pose these questions is the lever. Understand that mechanism and the other questions become approachable. Everything is connected, so the research deliberately spans more than computer science: physics, chemistry, biology, and philosophy all feed the same goal.

The near-term, concrete handle on all of this is the oldest one there is: how does a baby come to understand the world? Not by being trained on labeled data, but by predicting, being surprised, and slowly building an internal model through interaction.

## The bet

Today's AI is built by stacking abstractions: neural nets → deep learning → transformers → agents → orchestration. Each layer solves real problems and inherits every assumption from the layers below. Almost nobody building on top is asking whether the foundation is right. They are optimizing within the paradigm.

This project digs the other way. The current stack rests on assumptions that are rarely questioned:

- Digital binary computation
- Sequential token processing
- Massive scale as a substitute for architectural insight
- Language as both input and internal representation
- Separation of compute and memory (the von Neumann split)

The wager is that **representation, not scale, is the lever for general learning**, and that the substrate itself may be a ceiling rather than a detail. If even one of these inherited assumptions is a fundamental bottleneck, then understanding how learning actually works from first principles becomes the thing that matters.

## A taste of how we think

The sharpest one-liners live in [`personal-notes/key-insights.md`](personal-notes/key-insights.md), each backed by a full note. A few, to set the tone:

> The universe doesn't come with labels. We bring them and forget we brought them. — [`consciousness-and-the-label-problem`](research/consciousness-and-the-label-problem.md)

> A goal isn't a different kind of thing from a representation — it's a representation that points at *what to steer toward*, learned from the environment, not installed. — [`goals-as-learned-representation`](research/goals-as-learned-representation.md)

> "Shut up and calculate" is how working math buries a broken foundation. Predictions improving is evidence the model works, not that the foundation is right. — [`foundations-buried-by-working-math`](research/foundations-buried-by-working-math.md)

> The brain is 1,000–10,000× more energy efficient than GPUs — not from better engineering, but a different paradigm. The gap may not close within the current substrate. — [`energy-cost-of-intelligence`](research/energy-cost-of-intelligence.md)

Start anywhere: [what intelligence even is](research/intelligence.md), [whether it needs a brain](research/goals-as-learned-representation.md), [why we inherited the tools we did](research/inherited-tools.md), [finding structure vs. understanding it](research/grokking.md).

## Why we do it this way

- **First principles, always.** Every concept is explained from scratch. No jargon without explanation, no borrowed complexity. If something can't be explained simply, we don't understand it well enough yet — and we say so.
- **Every idea owes a way it could be wrong.** Conviction is fine; unfalsifiable conviction is not. The most valuable move is turning an argument into something testable (see the [Einstein–Bohr story](research/bell-theorem-and-nonlocality.md) for what 30 years of un-testable debate costs).
- **Show the work.** Dead ends and revisions stay in the record. The reasoning matters more than the conclusion.
- **Minimal.** No templates, no boilerplate, no scaffolding for its own sake. Notes link to notes; experiments test one idea at a time.

## How this project could be wrong

Stating the failure conditions up front is more useful than defending the thesis later. Honest ways this whole thing could be a mistake:

- **Scale might just win.** The "inherited assumptions are bottlenecks" claim is conviction, not proof. It is entirely possible that more scale and current architectures reach general intelligence and the foundational critique turns out to be romantic.
- **First principles can become reinventing the wheel.** Refusing to inherit anything is a great way to feel original while moving slowly and re-deriving things the field already knows. The line between "questioning foundations" and "ignoring hard-won knowledge" is real, and easy to get wrong.
- **It's early and unproven.** There is a lot of theory here and, so far, few experiments. Ideas that haven't been tested are just opinions held confidently.
- **"Everything is just a label" can become its own dogma.** The observation that fundamental concepts are observer-applied is powerful — and also seductive enough to over-apply until it explains everything and therefore nothing.
- **The baby analogy might mislead.** Modeling intelligence on human development bakes in human assumptions, which is exactly the kind of inheritance this project claims to avoid.

If any of these is fatal, the work of understanding learning from the ground up is still not wasted — but we would rather find that out fast than slowly.

## P0 target

An online learning system that continuously learns, integrates memory, and can understand analog clocks, the concept of time, and draw pictures of telling time accurately. Time is the first real test because understanding it cleanly separates *learning sequence* from *learning duration* — and that distinction reaches all the way down to the substrate question.

## Open questions (come argue)

If any of these keep you up at night, you're who this is for:

- Does intelligence need a brain at all, or is it just goal-directed competency under change? (cells, plants, collectives)
- Is a goal a learned representation rather than an installed drive — and what is the *minimal seed* that lets the first goal form?
- Is today's AI in its own "shut up and calculate" phase: benchmarks climbing on an unexamined foundation?
- Can a digital computer host a representation that genuinely *generalizes* — or do energy, parallelism, and the difference between *simulated* and *physical* time eventually force a different substrate?
- Why is the brain thousands of times more efficient — engineering, or paradigm?
- Is representation, not scale, the real lever for learning from few examples?

## Want in?

The priority is **debate and new ideas first, experiments second** — and the second is what keeps the first honest.

- **To argue an idea:** open a GitHub Issue or Discussion. One norm, strictly held: *every claim owes a way it could be wrong.* State the claim, why it might be wrong, and what would distinguish it from the alternative. Arguments that can't fill that third part are the ones we're trying to avoid.
- **No jargon-dropping.** Explain it from first principles or don't use it. That's the bar for everyone, including the author.
- **Come for the questions, not the credentials.** The interesting people here are the ones fascinated by the open questions above, whatever they do for a living.

## Repository

A research workspace and Obsidian vault — for organizing knowledge, linking ideas, and running small experiments. Not the final production codebase.

```
research/          # Research notes, paper summaries, and linked concepts
personal-notes/    # Motivation and the sharpest one-line insights
experiments/       # Coding experiments and proofs of concept (one idea each)
assets/            # Images, diagrams, and media referenced in notes
```
