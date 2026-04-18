---
date: 2026-03-28
tags: [complexity, entropy, information-theory, randomness, foundations]
sources:
  - "Kolmogorov, A.N. — On Tables of Random Numbers (1963)"
  - "Gell-Mann, Murray & Lloyd, Seth — Effective Complexity (1996)"
  - "Shannon, C.E. — A Mathematical Theory of Communication (1948)"
---

# Entropy Is Not Complexity

## The Common Conflation

Entropy increases over time. Disorder feels like complexity. So complexity must increase over time.

This is wrong. Entropy and complexity are different axes and can move in opposite directions.

## Two Definitions of Complexity That Contradict Each Other

**Kolmogorov complexity** — the length of the shortest program that produces a string:
- `000000000000000000` → short program ("print 0 eighteen times") → low complexity
- `10110010111001101...` (random) → no compression possible, shortest program is the string itself → **maximum complexity**

By this definition: **random = maximally complex.**

**Gell-Mann's effective complexity** — the length of the description of the *regularities only*, excluding the random residue:
- Random noise: short schema ("it's random, distribution X") → **low effective complexity**
- DNA, a brain, a city: long schema of non-trivial structure → **high effective complexity**

By this definition: **random = minimally complex.**

These are not reconcilable. They measure different things.

## Gell-Mann's Framework is Anthropocentric

Effective complexity splits a thing into signal (schema) and noise (random residue). It only counts the signal. The argument: the random part doesn't contain useful structure.

But "useful structure" implies an observer with goals. The random part is called noise because *we* can't model it further — not because it lacks structure. This is an epistemic limitation dressed up as an ontological fact.

A sufficiently powerful observer might find the "random residue" to have deep structure we simply can't see yet.

## Is Randomness Real or Epistemic?

In classical physics: the universe is deterministic. "Random" always means we lack information. A coin flip is random to us, not to a perfect physics simulator.

In quantum mechanics: Bell's theorem rules out certain hidden variable theories. Randomness may be genuinely ontological at the quantum level.

Historically, many things that appeared random turned out to have structure once the right lens was found:
- Chaos theory: deterministic systems that look random
- Fractals: infinite apparent complexity from a 3-line formula
- Prime numbers: look random, deep structure still being uncovered

"Random" has repeatedly been a placeholder for "pattern we haven't found yet."

## What Happens to the Entropy-Complexity Picture

If Kolmogorov is right:
- Heat death (maximum entropy, pure randomness) = maximum complexity
- Structured things (crystals, DNA) = less complex, because compressible
- The universe trending toward disorder is trending toward more complexity, not less

If Gell-Mann is right:
- Complexity peaks at intermediate entropy — the "edge of chaos"
- Life, neural computation, language live here
- Heat death = minimum effective complexity

Both capture something real. The choice of definition depends on what you're trying to understand.

## Complexity May Be Observer-Relative

The deeper question: is complexity a property of the world, or a property of the relationship between the world and an observer trying to model it?

If the latter, then "this is random, therefore low complexity" is always a statement about the observer's limits — not the thing itself. Complexity is not intrinsic; it's relational.

This has direct consequences for any learning system. What looks like noise to one model may be signal to a better one. The apparent complexity of a stimulus depends entirely on the representational capacity of the system perceiving it.

## Relevance to Abby

A learning system trained to compress experience will treat its residual — whatever it can't model — as noise. But that residue may contain the most important structure. The question is how to avoid permanently discarding what can't yet be described.

See also: [[intelligence]] [[brain]] [[information_processing]] [[grokking]]