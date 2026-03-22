---
date: 2026-03-09
tags: [language, communication, animals, foundational]
sources:
  - https://www.youtube.com/watch?v=RKK7wGAYP6k
  - https://youtu.be/Hve8_iSDD-o?si=sZBpRTxyVmQYLuIq
  - https://youtu.be/hph9OeKjg3w?si=lsc2Pj6ZwQUuQ7xI
  - https://www.projectceti.org/
---

# Language and Communication

## Core Idea

All communication media — baby cries, whale clicks, body language, speech, writing, math notation — are forms of language in the abstract sense: structured systems for transferring state between entities. They differ in bandwidth, precision, and abstraction capability, but serve the same fundamental purpose.

## Language Shapes Thought (Sapir-Whorf)

The language you speak doesn't just express your thoughts — it influences what you can think. The weak version of the Sapir-Whorf hypothesis has solid evidence:
- Languages without left/right (only cardinal directions) produce speakers with better spatial orientation
- Grammatical gender influences object perception
- Number of color terms affects how quickly speakers distinguish colors
- English forces tense specification, Mandarin doesn't — these shape what's easy to think about

Implication: the representation system chosen for an artificial learner isn't neutral. It actively constrains what the system can learn.

## Origin of Grammar

Two major camps, unresolved:
- **Chomsky's Universal Grammar** — innate, hardwired grammar structure; babies parameterize it from exposure. Nativist/genetic.
- **Emergentist view** — grammar emerges from social interaction, pattern recognition, and statistical learning. No innate module needed. Connects directly to [[emergence]].

## Animal Communication

A spectrum from pure signal to structured language:
- **Baby crying** — no structure, but communicates state effectively
- **Animal signals** — structured, some combinatorial, possibly no abstraction
- **Sperm whale codas** — rhythmic click sequences with combinatorial structure, clan dialects, individual identity markers. Possibly somewhere between signal and language. Project CETI is using ML to decode whether this has syntax and semantics.
- **Human language** — full recursion, abstraction, displacement, grammar

Open question: is whale communication qualitatively different from language, or a different point on the same spectrum?

### Animals That Mimic Human Speech

Many unrelated species can produce human-like speech sounds — parrots, corvids, mynahs, elephants (trunk in mouth to shape sounds), beluga whales, orangutans, harbor seals. Alex the African Grey could answer novel questions about color/shape/quantity with ~80% accuracy — hard to explain as pure mimicry.

But none demonstrate generative grammar — combining words in novel ways for novel ideas. The motor control for producing speech sounds isn't rare. What's rare is the cognitive architecture for abstract, compositional, recursive language. Many animals cracked the medium; none cracked the system.

## Limitations of Human Language

- **Bandwidth** — ~150 words/minute while the brain processes millions of signals per second. Language is a straw draining an ocean.
- **Encoding overhead** — effort spent on spelling, grammar, syntax, word order has zero information content. The machinery of encoding consumes cognitive resources unrelated to the actual idea.
- **Ambiguity** — relies on shared context to resolve meaning
- **Linear bottleneck** — thought is parallel and multi-dimensional, language serializes it into a single stream
- **Lossy compression** — listener decompresses into their own mental model, never exact
- **Cultural/linguistic bias** — language filters reality (Sapir-Whorf)
- **Discrete symbols for continuous reality** — carves the world into categories ("red" vs "orange") but reality is a spectrum. Connects to [[emergence]] and information processing themes.

## Was Language a Good Choice?

Language wasn't "selected" — it emerged from proto-communication (grunts, gestures, facial expressions) over hundreds of thousands of years. Nobody designed it. So asking "did we make a mistake" is like asking "did evolution make a mistake selecting legs" — there was no selection event, just accumulated drift.

**What language is good at despite its flaws:**
- **Abstraction** — you can talk about things that don't exist, haven't happened, or are hypothetical. No animal communication can do this. This is arguably what made humans dominant.
- **Compositionality** — finite words, infinite sentences. Novel ideas from existing pieces.
- **Persistence** — language can be written down. Civilization's cheat code — knowledge accumulates across generations.

**Why "efficient" alternatives fail for humans:**
Every attempt at efficient languages (Lojban, formal logic, programming languages) is terrible for human communication. The "overhead" — redundancy, ambiguity, irregular verbs — actually provides error correction and flexibility. The "inefficiency" helps listeners reconstruct meaning even when they miss parts. The ambiguity and social wrapping are features, not bugs — they grease social interaction.

## Alternative Communication: Spatial Rather Than Sequential

What if communication was parallel and visual rather than sequential and symbolic?

Rough sketch: instead of serializing thoughts into words, place objects in a shared space where position encodes certainty, size encodes importance, color encodes emotional tone, and line types encode relationship strength. A diagram conveys structural relationships at a glance that take paragraphs to describe in words.

This is what diagrams, whiteboards, maps, and dashboards already do — we use them when words fail because spatial representation carries structural information that sequential language can't. Obsidian's graph view is a primitive version of this.

**Where it breaks down:**
- Abstract concepts without spatial metaphors ("justice," "maybe," "irony") are hard to place
- Temporal sequences (stories, processes) don't map naturally to 2D space
- Shared conventions for position/color/size start looking like grammar again

Core idea: **parallel visual processing instead of sequential symbolic parsing.** Humans already do this informally — it's just never been formalized as a primary communication medium. A genuinely difficult problem to solve.

## Relevance to Abby

Two separate problems:
1. **Internal representation** — how does Abby think/process? Doesn't need to be human language. Could be something entirely new. If you build the system to communicate in human language from the start, you import all these limitations into its core.
2. **External interface** — how does Abby communicate with humans? Must be human language (text, speech, visuals) because that's what humans operate in.

The translation layer between internal representation and human language is a key design challenge. For a non-human system, the constraints are completely different — it could natively process structured, multi-dimensional, uncertainty-weighted representations without serializing into words.

## To Explore Later

- How did language structure/grammar originally emerge in human evolution?
- Deeper dive into Project CETI findings
- What properties would an ideal internal representation have (non-linguistic, continuous, multi-dimensional)?
- How babies transition from pre-linguistic understanding to language
- Could a spatial/visual communication medium be formalized? What would the "grammar" look like?
- Humming and music as higher-bandwidth channels for emotional state vs lower-bandwidth for precise content
