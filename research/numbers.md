---
date: 2026-03-09
tags: [numbers, information-processing, foundational]
sources:
  - https://youtu.be/FmLIGN8ZGdw?si=EHJuDJcFmhFGugH_
  - https://youtu.be/beakj767uG4?si=ZYUTfQPTnkKPVFNB
  - https://youtu.be/5TkIe60y2GI?si=sLylXi3p6EjkFfVF
  - https://claude.ai/share/aa67bb61-cddf-44ae-999c-9952bc44d10e
---

# Numbers

Numbers are a human-invented concept — a framework for quantifying and reasoning about the world. Over centuries, each new type of number was introduced to solve a problem the previous type couldn't handle. This layering is worth examining critically.

## The Number Hierarchy

**Natural numbers (1, 2, 3, ...)** — counting. The most intuitive. How many things are there?

**Whole numbers (0, 1, 2, 3, ...)** — added zero. The concept of "nothing" as a quantity was not obvious — many civilizations didn't have it.

**Integers (..., -2, -1, 0, 1, 2, ...)** — added negatives. Introduced to handle debt, direction, and subtraction beyond zero.

**Rational numbers (1/2, 3/4, -7/3, ...)** — ratios of integers. Introduced for division. Any number expressible as p/q where q ≠ 0. Covers fractions and repeating decimals.

**Irrational numbers (√2, π, e, ...)** — cannot be expressed as a ratio of integers. Discovered by the Greeks (√2 from the diagonal of a unit square). Their existence was initially considered a crisis — it broke the Pythagorean worldview that everything was ratios.

**Algebraic irrationals (√2, φ, ∛5, ...)** — irrational but can be "caught" by polynomial equations with rational coefficients. √2 solves x² - 2 = 0. The golden ratio φ solves x² - x - 1 = 0. Irrational but still within reach of algebra.

**Transcendental numbers (π, e, ...)** — cannot be captured by any polynomial equation with rational coefficients. They transcend the entire machinery of algebra. Almost all real numbers are transcendental, yet we can only name a few. Known examples: π, e, eᵖ, ln(2), sin(1), the Champernowne constant (0.123456789101112...). Surprisingly, we can't even prove whether π + e or πe are transcendental.

**Real numbers** — the entire continuous number line. Rationals + irrationals together. Fills in "all the gaps."

**Complex numbers (a + bi)** — introduced i = √(-1) to solve equations like x² + 1 = 0. Extends the number line into a 2D plane. Essential in physics, quantum mechanics. The Fundamental Theorem of Algebra says every polynomial has a solution in complex numbers — the number system expansion stops here.

**Computable numbers** — real numbers that can be computed to arbitrary precision by a finite algorithm. Almost all real numbers are *not* computable (there are uncountably many reals but only countably many algorithms). We can only ever work with computable numbers, yet they're a vanishingly small subset of all reals.

## The Number Hierarchy as Historical Scar Tissue

Each layer was added to patch a limitation of the previous one. Each addition felt unnatural at first (zero, negatives, irrationals, imaginary numbers were all controversial when introduced — the Pythagoreans reportedly drowned the man who proved √2 was irrational). Each eventually became indispensable.

The categories — natural, integer, rational, irrational, algebraic, transcendental — aren't a clean taxonomy of nature. They're historical artifacts. Each marks a moment where the existing system broke and was patched. The entire rational/irrational/transcendental classification is really just measuring distance from integers. Integers are "home base," everything else is ranked by how far it strays.

But reality is the opposite — almost all numbers are transcendental, and integers are the rare, special freaks. π isn't inherently weird. It's only weird relative to integers.

## Pi, Circles, and Irrationality

Pi's irrationality is a property of the number itself (proven by Lambert, 1761), not a physical limitation. The impossibility of drawing a perfect circle is a separate, purely physical constraint.

Key insight: for any circle, the diameter and circumference can't both be exact rational numbers simultaneously (since circumference = π × diameter). If one is "clean," the other must be irrational. The irrationality has to live somewhere.

In a relative system, this wouldn't matter — you'd just say "the circumference is π of the diameter" and treat that ratio as the complete description. The "problem" of irrational numbers is partly an artifact of insisting on absolute decimal representation.

## Euler's Number (e)

e ≈ 2.71828... emerges from compound interest: split 100% interest into infinitely many compounding steps and the result converges to e. It appears throughout nature wherever something changes at a rate proportional to its current state — population growth, radioactive decay, cooling curves, spiral shells, hanging chains (catenary curves). If π is the constant of shape, e is the constant of continuous change.

e is proven irrational (and transcendental) via an elegant squeeze argument: assume e = p/q, multiply the factorial series by q!, and the remainder is forced to be a whole number between 0 and 1 — which is impossible.

## The Golden Ratio (φ)

φ = (1 + √5) / 2 ≈ 1.618... is the ratio where the whole relates to the large part as the large part relates to the small part. It is irrational but **not transcendental** — it solves x² - x - 1 = 0, making it algebraic.

The Fibonacci sequence (1, 1, 2, 3, 5, 8, 13...) naturally converges to φ in the ratios of consecutive terms. φ is the "most irrational" number — hardest to approximate with fractions — which makes it nature's optimal "avoid clumping" angle for seed packing in sunflowers, pinecones, and spiral growth.

## Curvature and Transcendence

Arc lengths of curves are almost always irrational and frequently transcendental. The arc length formula ∫√(1 + f'(x)²)dx involves integrating a square root of a varying quantity — summing infinitely many tiny hypotenuses with different ratios of sides. This destroys rationality.

The arc length of one period of a sine wave ≈ 7.6404 is proven transcendental (via Schneider's 1937 theorem on elliptic integrals). Straightness is the exception that permits rationality; curvature is the rule that destroys it.

## Do We Really Need Absolute Numbers?

We don't encounter exact "3" in the universe. Even "3 bananas" involves variance in size, shape, weight. Numbers encode absolute position on a line, but what we actually care about is relationship to context — scale, precision, comparison.

3 cm matters for a blueberry. 3 cm is meaningless for measuring Earth's radius. The number is the same; the relevance is entirely contextual. Human perception already works this way — the Weber-Fechner law shows we perceive differences proportionally (doubling from $100→$200 feels the same as $10,000→$20,000).

Alternative approaches explored:
- **Ratio-based primitives** — everything is a comparison, never absolute. Music intervals work this way (ratios, not frequencies).
- **Scale-aware representations** — numbers as tuples: (value, scale, tolerance).
- **Category-theoretic thinking** — objects don't matter, only relationships between them.
- **Information-theoretic** — a measurement is an answer to a question. Encode how many bits of distinction you're making, not pretend infinite precision.

## Logarithms

Invented by Napier (1614) to turn multiplication into addition. For 400 years, log tables were the most important computational tool on Earth.

Deeper significance: logarithms formalize relative thinking. They convert ratios into differences, which is how human perception naturally works (decibels, Richter scale, pH, stellar magnitude). Shannon defined information using logarithms — log₂(outcomes) = bits — because information should be additive when possibilities multiply.

**Limitation:** Logarithms are opinionated. They're biased toward ratios. When two numbers are nearly identical proportionally but the tiny gap matters (two stars 4.000000 vs 4.000001 light years away), logarithms actively hide the important difference.

**In a ratio-native system, logarithms are ~80% unnecessary.** They exist as a bridge between additive and multiplicative worlds. If your system starts multiplicative, you don't need the bridge. The ~20% that survives: counting depth of compounding ("A is 3 levels of tripling away from D").

## The Ramanujan -1/12 Problem

Ramanujan's claim that 1 + 2 + 3 + ... = -1/12 illustrates how far this layering can go. The sum diverges under standard arithmetic. To get -1/12, you need regularization techniques (analytic continuation of the Riemann zeta function) — introducing new mathematical machinery and assumptions. The result is useful in physics (string theory, Casimir effect) but the question remains: are we discovering something real, or are we building layers of abstraction so deep that the assumptions underneath become unexplainable?

## The Deeper Question

Every mathematical tool we've built — logarithms, trigonometry, calculus — is partly solving real structural problems and partly compensating for the limitations of our chosen representation. Which parts of existing mathematics reflect genuine structure in reality, and which parts are just patches over bad design choices in our number system?

Even in a ratio-based world, you can't escape π — any system capable of comparing magnitudes will rediscover it. But you can build a system where π isn't "weird," where it's just another relationship among equals, and integer ratios are treated as a curious coincidence rather than the definition of "normal."

## To Explore Later

- Discrete vs continuous — is reality fundamentally discrete (countable) or continuous?
- Why does the complex number plane show up everywhere in physics?
- What would a number system designed for a learning system look like?
- Projective geometry, category theory, and constructive mathematics as alternative foundations
- Pythagorean hodograph curves — engineered curves with rational arc lengths
