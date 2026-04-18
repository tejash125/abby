---
date: 2026-03-28
tags: [foundations, abstraction, mathematics, truth, epistemology, deep-learning, intelligence]
sources:
  - "Peano, G. — Arithmetices Principia (1889)"
  - "Russell & Whitehead — Principia Mathematica (1910-1913)"
  - "Gödel, K. — On Formally Undecidable Propositions (1931)"
  - "Kuhn, T. — The Structure of Scientific Revolutions (1962)"
---

# Inherited Tools

## The Starting Claim: Math is Invented

Symbols are invented. 1, 2, 3, +, = — all conventions, agreed upon, not discovered from nature. The question is whether the *relationships* between those symbols are also invented, or whether they capture something real.

The strongest version of the formalist position: even "discrete quantity" is an abstraction we imposed on a world that doesn't come in clean discrete units. The world is continuous, fuzzy, contextual. We invented discreteness as a useful fiction and built arithmetic on top of it.

## Counting Was Never About Stones

"1 stone + 2 stones = 3 stones" loses information immediately:
- What if one stone is half the size of the others?
- When does a pebble become a stone? A stone become a rock?
- What if one is cracked — is it one stone or two?

Before you can count, you have to decide what *counts as one thing*. That categorical decision is prior to arithmetic and is not made by mathematics — it's made by the observer, for a purpose.

**The actual origin of counting:** Trade and resource allocation. When humans exchanged goods with strangers, they needed a system that worked without shared context. You can't say "give me the bigger pile" to someone you don't trust. You need a neutral, agreed-upon unit. Counting solved the social coordination problem of exchange between people who couldn't rely on shared judgment.

Arithmetic wasn't invented to describe reality accurately. It was invented to solve a specific, narrow, practical problem — and then generalized far beyond that context and treated as fundamental truth.

The cost: an entire civilization of thought built on a foundation designed for counting grain. That foundation shapes what we can think, because the tools we inherit push us toward discrete, countable, separable representations of a world that isn't actually like that.

## All Knowledge Rests on Unjustified Axioms

**The Münchhausen trilemma:** Ask "why is X true?" and you get one of:
1. An infinite chain of justifications (infinite regress)
2. A circular argument
3. A bedrock axiom you simply accept

All knowledge eventually stops at option 3. You cannot justify your foundations from within the system built on them.

Gödel formalized this for mathematics specifically: any sufficiently powerful formal system contains truths it cannot prove from within itself, and cannot prove its own consistency. The foundation is always, at some level, just accepted.

**Truth, then, looks like:** a statement is true within a system if it follows from that system's axioms. Whether the axioms themselves are "true" is a question the system cannot answer. There is no view from nowhere.

Old axioms can turn out to be wrong — or rather, approximate. Euclid's parallel postulate held for millennia. Non-Euclidean geometry dropped it and turned out to describe spacetime better. The old axiom wasn't *wrong* exactly; it was a useful approximation, not a truth.

## The Intelligence Problem

The most uncomfortable instance of this pattern: we are building toward "superintelligence" without agreeing on what intelligence is. The word has been used, defined, redefined, and argued over for a century. And yet entire research programs, companies, billions of dollars, and policy decisions are organized around it.

We're not optimizing toward a goal. We're optimizing toward a *proxy* for a goal we never fully specified — benchmark scores, loss functions, human preference ratings — and calling the proxy the goal. (Goodhart's Law at civilizational scale.)

The humans defining what intelligence should look like are themselves intelligences shaped by their own assumptions, culture, and cognitive limits. We can't step outside to get a clean view.

## Do Transformers Have Axioms?

Humans reason axiomatically — but mostly implicitly. Foundational assumptions (causality, object permanence, basic quantity sense) are installed before a child can question them and function as axioms that never get examined.

Transformers do not have axioms in the same sense. What they have:

**Architecture as prior** — attention mechanisms, residual connections, positional encoding are assumptions about structure baked in by the designer before training. These are the builder's axioms, not the model's.

**Training data as implicit ground truth** — whatever is statistically dominant in training data functions as a baseline assumption. Not adopted axiomatically — just learned to pattern-match toward.

**Learned circuits** — mechanistic interpretability reveals that models develop internal circuits that consistently implement specific computations. These function like soft axioms from the outside. But they are opaque to the model itself, not verified for consistency, and can conflict with each other.

**The key difference from human axiomatic reasoning:** A human can examine their axioms, argue about them, revise them, extend them deliberately. The framework is at least partially transparent to the reasoner. A transformer's implicit axioms are invisible to itself. It cannot detect when two of them conflict, cannot deliberately extend them, has no mechanism to distinguish "this updates my foundation" from "this is a local fact."

**Can a transformer extend its framework as it deals with life?**

Current transformers: no. Weights freeze after training. In-context learning is a workaround — new premises in the context window are reasoned from — but they evaporate when context ends. Nothing updates foundationally.

For a genuinely online learning system, genuine axiomatic extension would require:
- Persistent, writable long-term memory
- A consistency mechanism to check new beliefs against existing ones
- A way to distinguish foundation-updating events from ordinary learning

The third is hardest. Humans do it through **surprise and reflection** — something violates expectation strongly enough that the assumption is questioned, not just the instance. No current architecture has a good model of this.

**Transformers behave as if they have axioms. They do not actually have a consistent foundational framework they reason from.** The training objective (predict next token) does not require internal consistency — just plausible output distributions.

## The Pattern

Counting, logic, truth, intelligence — all foundational concepts that were:
1. Invented or defined for narrow, practical purposes
2. Generalized far beyond their original scope
3. Adopted so widely that questioning them became costly
4. Treated as discovered rather than invented

The tools we inherit shape what questions we can ask. Inheriting discrete arithmetic makes continuous cognition harder to conceptualize. Inheriting benchmark-based intelligence definitions makes genuine intelligence harder to build toward.

## Relevance to Abby

A baby's first experience of quantity is not counting — it is more/less, bigger/smaller, closer/farther. Continuous and relational, not discrete and absolute. Discrete counting arrives later, taught, as a social tool layered on top of continuous intuition.

The foundational design question for Abby: which inherited tools to adopt, which to question, and which to replace. The assumptions that get baked in earliest will shape everything above them. The most important design decisions may be about what *not* to assume.

See also: [[numbers]] [[intelligence]] [[grokking]] [[brain]]