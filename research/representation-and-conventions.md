---
date: 2026-06-30
tags: [representation, conventions, epistemology, meaning, truth, philosophy-of-science]
sources:
  - https://plato.stanford.edu/entries/convention/
  - https://iep.utm.edu/poi-math/
  - https://en.wikipedia.org/wiki/Two_Dogmas_of_Empiricism
  - https://plato.stanford.edu/entries/scientific-underdetermination/
  - http://www.scholarpedia.org/article/Symbol_grounding_problem
  - https://en.wikipedia.org/wiki/Signaling_game
  - https://www.academia.edu/1192679/Luc_steels_the_talking_heads_experiment_and_cognitive_philosophy
  - https://iep.utm.edu/truth/
  - https://activeinference.github.io/papers/process_theory.pdf
---

# Representation and Conventions

How does a mind come to *understand* anything, and how does a group ever agree
on what things mean? This note gathers what people outside this project have
worked out about two questions: (1) what a representation is and how a stand-in
gets to be *about* the world, and (2) how conventions form and how we judge
whether one is "right." It is the outside-knowledge companion to the
philosophy we are assuming in `experiments/experiment_1`.

## Part 1 — Representation: a stand-in that is *about* something

A **representation** is a stand-in: something inside a system that varies along
with something outside it, so the system can act on the stand-in instead of the
thing itself. A fuel gauge is a stand-in for how much petrol is left.

The hard part is not the varying-together. It is **aboutness** — what makes the
gauge be *about* the petrol rather than just a needle that happens to move? In
philosophy this directedness-at-something is called **intentionality** (a
technical word meaning "aboutness," nothing to do with intending). A pile of
symbols pushed around by rules is not automatically about anything.

### The symbol grounding problem

Stevan Harnad (1990) sharpened this into the **symbol grounding problem**: if
every symbol is defined only using other symbols, the whole system is a
dictionary with no pictures — you can look up a word forever and never reach the
world. Meaning has to bottom out somewhere outside the symbol-shuffling. His
proposed bottom: **sensorimotor grounding** — some symbols are tied directly to
what the system senses and does, and the rest are built on those.

This is the same shape as the understanding claim in experiment_1: a handed-down
name becomes real understanding only when it gets anchored to a regularity the
learner caught on its own. Grounding *is* that anchoring. See
[[foundations-buried-by-working-math]] for the related point that the chain of
justification has to stop somewhere.

### Two cheaper ways to think about aboutness

- **The intentional stance** (Dennett): maybe "aboutness" is not a special inner
  substance at all. We *treat* a system as having beliefs about X because doing
  so predicts its behavior well. Aboutness becomes a useful description from the
  outside, not a thing you have to manufacture inside. This matters for Abby: we
  may not need to *install* meaning, only build a system whose behavior is best
  described as being about the world.
- **Prediction as the engine** (predictive processing / the free-energy
  principle, Friston): treat the system as constantly guessing its next sensory
  input and correcting when wrong. On this view a representation just *is* the
  internal model that generates the guesses, and perception is the model being
  corrected by reality. This is exactly experiment_1's Engine 1, arrived at from
  neuroscience. See [[physics-as-perception]] and
  [[goals-as-learned-representation]].

### Structure, not stuff

One more useful idea: maybe what a good representation captures is not the
*intrinsic nature* of things but the **relationships** between them. You never
get to the "what it is in itself"; you get the pattern of how things relate and
change. (This is the epistemology side of **structural realism**; the physics
side is in [[foundational-blocks-universe-and-abby]].) This lines up with the
experiment_1 proposal that representation = the learned relationships between
predictors, over continuous values, with time built in.

## Part 2 — Conventions: the agreed layer

Some of what we "know" is not read off the world; it is **agreed**. No amount of
watching the sky tells you to call one side "east." These agreed parts are
**conventions**.

### Hume and Lewis: a convention is a self-holding coordination habit

David Hume's picture: a convention arises when people sense a common interest and
fall into step without any explicit contract — two men rowing a boat sync their
strokes with no agreement signed. It holds itself up: *you do it because they do,
and they do it because you do.*

David Lewis (1969) made this precise with game theory (the study of choices that
depend on others' choices). A **coordination problem** is one where several
arrangements would suit everyone equally — the only thing that matters is that we
all pick the *same* one (which side of the road to drive on). A **convention** is
one such arrangement that holds because:

1. nearly everyone follows it,
2. everyone expects everyone to follow it,
3. everyone prefers to follow it *given that the others do*, and
4. some other arrangement would have worked just as well.

Two pieces are doing the heavy lifting:

- **Common knowledge** — not just that everyone knows the rule, but everyone
  knows that everyone knows, and so on. The expectation has to be mutual and
  visible, or it does not stabilize.
- **Salience** — when several options would all work, the one that *stands out*
  gets picked (meet "at the obvious place at noon"). Salience can come from
  precedent, from being explicitly named once, or from something just looking
  like the natural choice.

### How a convention forms from scratch (the buildable version)

This is the part most relevant to Abby, because it has been *simulated*, not just
argued about:

- **Signaling games** (Lewis, then Skyrms): a sender sees a state and emits a
  signal; a receiver acts on the signal. When they win together, both reinforce
  what they did. With nothing but this reward-and-repeat loop, a *shared code*
  emerges — signals come to "mean" states. No built-in dictionary, no salience
  even required; plain reinforcement is enough. Meaning is the surviving
  equilibrium.
- **The naming game / Steels' "Talking Heads"**: a population of agents play
  pairwise "what do you call that?" games about things they actually see through
  cameras. Through purely local interactions — no central authority — they
  converge on one shared vocabulary. This is convention formation as an
  *emergent* phenomenon, grounded in shared perception. See [[language]] and
  [[emergence]].

The lesson: a convention is not an arbitrary decree handed down. It is a stable
agreement that *self-organizes* out of many agents trying to coordinate, each one
running the same humble loop (act, see if it landed, adjust). That is the *same*
loop as Engine 1. So conventions (Engine 2's content) are themselves built by
many copies of the Engine-1 machinery talking to each other — which supports the
experiment_1 stance that there is no separate "trust module" or "convention
module"; it is one mechanism, networked.

### Conventionalism: some "laws" are choices

Poincaré argued that parts of science we take as discovered are actually
*chosen* — geometry, units, what counts as "simultaneous." Not arbitrary
(experience pushes hard on the choice), but not forced either; we adopt them for
simplicity and fruitfulness, and could in principle have chosen otherwise. The
logical positivists ran with this. The takeaway for Abby: the line between
"fact" and "convention" is blurrier than it looks — much of the castle is
agreed-upon scaffolding that the world merely fails to knock down.

## Part 3 — How do we know a representation or convention is *right*?

There is no way to step outside all our representations and check them against
bare reality. So "right" gets defined three classic ways:

- **Correspondence** — right means *matches the world*. Intuitive, but you can
  never get outside your own representations to verify the match, which is the
  standing complaint against it.
- **Coherence** — right means *fits with everything else you hold*. Good for
  catching contradictions, weak on its own (a tidy fairy tale can be perfectly
  coherent).
- **Pragmatic** (Peirce, James, Dewey) — right means *acting on it works*: it
  predicts, it lets you intervene successfully. This is the one that matches
  experiment_1's "the world votes." A representation earns its keep by paying out
  in correct anticipation; one that keeps being wrong gets dropped.

A modern sharpening of the pragmatic line: a good model is one that **compresses**
the past and **predicts** the future. Being "right" is gradable — measured by how
much surprise the model removes — not a yes/no stamp. This dissolves the
"correspondence is uncheckable" worry: you are not checking against bare reality,
you are checking whether the next moment surprised you.

### Quine: it is a web, judged as a whole

Quine's "Two Dogmas of Empiricism" (1951) attacks the clean split between
convention (true by meaning) and fact (true by the world). His picture: all our
beliefs form **one connected web** that meets experience *as a whole*. When
something doesn't fit, we can fix the web in many places — we usually protect the
core (logic, math) because changing it is expensive, and revise the edges first.
No single belief is immune to revision, and none is purely convention or purely
fact; they sit on a continuum of *how willing we are to give them up.*

Two consequences carry straight into this project:

- **Underdetermination**: the evidence never picks out exactly one theory; more
  than one web can fit the same experience. So "right" is never fully forced by
  the data — taste, simplicity, and history do real work. (Same shape as
  Poincaré's conventionalism and as [[foundations-buried-by-working-math]].)
- Quine's web is the rigorous version of experiment_1's **castle**: floors held
  firm not because they are proven but because too much rests on them. "Right"
  = "the web keeps absorbing experience without having to tear out the core."

## Bottom line for Abby

- Representation = a stand-in whose *aboutness* comes from being grounded in what
  the system senses and does, and from earning its keep by predicting. We
  probably do not install meaning; we build the predict-and-correct loop and
  meaning is what that loop's internal states *become*.
- Conventions are not decrees. They self-organize from many agents each running
  the same humble act-check-adjust loop, coordinating until one shared
  equilibrium survives. This is direct evidence for "no separate trust module."
- "Right" is best taken pragmatically and holistically: a representation or
  convention is right to the extent that acting on it keeps removing surprise,
  and the whole web keeps absorbing experience without breaking its core. There
  are no bare facts to check against — only the world declining to surprise us.

## Open threads

- Signaling games produce shared codes with *no* built-in salience. Does that
  mean salience/relevance is fully emergent for Abby too, or is some minimal
  "what to attend to" still primitive? (Ties to experiment_1's open question on
  relevance.)
- Pragmatic "right" = predicts well. But a convention can predict nothing on its
  own (which side of the road is pure coordination). So Abby needs *two* senses
  of right: "predicts the world" (regularities) and "matches the group"
  (conventions). Are these one mechanism or two?
