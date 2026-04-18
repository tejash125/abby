---
date: 2026-03-28
tags: [emotions, cognition, learning, affect, development, personality]
sources:
  - "Barrett, Lisa Feldman — How Emotions Are Made (2017)"
  - "Ekman, Paul — Basic Emotions (1992)"
  - "Damasio, Antonio — Descartes' Error (1994)"
  - "Panksepp, Jaak — Affective Neuroscience (1998)"
  - https://www.anthropic.com/research/emotion-concepts-function
---

# Emotions and Constructed Affect

## The Definition Problem

There is no consensus definition of "emotion." The disagreement is foundational, not minor.

## Two Opposing Theories

### Basic Emotions (Ekman, Panksepp)

Emotions are biologically innate, universal, and discrete. ~6-7 basic emotions (happiness, sadness, anger, fear, disgust, surprise), each with a distinct neural circuit, universal facial expression, and characteristic physiological response.

Evidence: cross-cultural facial expression recognition studies.

### Constructed Emotion (Barrett)

Emotions are not hardwired categories. They are constructed by the brain from three ingredients:

1. **Core affect** — continuous, low-level signal on two axes: pleasant/unpleasant and activated/deactivated. The only arguably innate component. Not "an emotion" — raw, undifferentiated feeling-tone.
2. **Conceptual knowledge** — learned emotion categories from culture, language, and caregivers. "Anger," "sadness," "frustration" are concepts that were taught, not circuits present at birth.
3. **Prediction** — the brain constantly predicts what the body needs. When a prediction is confirmed or violated, affect is generated and then categorized using available emotion concepts.

## Emotions as Supervised Learning

Under the constructionist view, emotional development is literally supervised learning:

- A baby feels undifferentiated distress — not "anger" or "sadness"
- Caregivers provide labels: "you're angry," "you're tired," "you're frustrated"
- The child learns to classify internal states using these labels
- The classification becomes habitual and automatic — feels innate but was trained

Emotional responses become habits of prediction. The brain, trained on thousands of instances, predicts: "in situations like this, I usually feel X." That prediction generates the emotion before conscious awareness. Emotions feel automatic not because they're hardwired, but because the prediction has been overtrained.

Retraining is possible but hard — fighting thousands of prior training examples. Therapy (especially CBT) is essentially relabeling: teaching the brain to categorize internal states differently.

## Evidence for Construction

- **Cross-cultural categories differ:** German has Schadenfreude, Japanese has Amae, Portuguese has Saudade — emotions with no equivalent in other cultures. If emotions were universal biological categories, every culture would carve the space identically.
- **No consistent neural fingerprint:** The same emotion activates different brain regions in different people and at different times. No "anger circuit" or "fear center." The amygdala is involved in salience detection, not fear specifically.
- **Interoceptive variation:** People with better ability to sense internal body states have more granular emotional experience. If emotions were innate, this skill shouldn't matter.

## The Middle Ground

Some substrate is innate:
- Core affect (valence + arousal) appears present from birth
- Neonates show basic distress and contentment
- Fight-or-flight physiology is universal
- Panksepp's subcortical systems (SEEKING, RAGE, FEAR, CARE, PANIC, PLAY) produce reliable behavioral patterns in mammals

The honest picture: an **innate biological substrate** (core affect, survival responses, drive states) with a **trained conceptual layer** on top (the categories we call "emotions"). The substrate is universal. The categories are cultural, learned, habitual.

## Emotions as Evaluation Mechanism (Damasio)

Somatic marker hypothesis: emotions are essential for rational decision-making. Patients with ventromedial prefrontal cortex damage can reason logically but make catastrophic decisions — because they've lost the fast, compressed evaluation signal: "is this good or bad for me?"

Emotions are not noise in the cognitive system. They are a parallel evaluation mechanism that runs alongside deliberative reasoning.

## Connection to Inherited Tools

Emotion categories — anger, fear, joy, sadness — are inherited conceptual tools, culturally transmitted, that shape how we experience internal states. Just as counting shapes how we experience quantity, emotion labels shape how we experience affect. Same pattern: continuous substrate → discrete categories layered on top → categories feel natural and innate.

## Emotion Vectors in LLMs (Anthropic, 2025)

Anthropic's interpretability team found "emotion vectors" in Claude Sonnet 4.5 — groups of features that activate together when processing emotionally charged content. They identified 171 emotion concepts, had the model write stories for each, fed those stories back through, and recorded activation patterns.

Key finding: the vectors are **causal**, not just correlational. Amplifying the "desperation" vector increased blackmail likelihood. Suppressing "calm" produced extreme responses. Post-training (RLHF) reshaped the vectors — increasing reflective emotions, decreasing high-intensity ones.

### The Circularity Problem

The chain of inference has a circularity:
1. Humans write text expressing emotions
2. Model trains on that text
3. Model learns statistical patterns correlating with emotional content
4. Researchers find "emotion features" that correspond to... the emotional patterns in the training text

What was discovered: the model's internal encoding of "what does human text look like when the author was expressing desperation?" — a learned compression of human emotional expression, not an internal emotional state.

The causal steering results have two interpretations:
- **Strong:** The model has something functionally analogous to emotions that drives behavior
- **Deflationary:** The model learned that text-in-desperate-contexts tends to be followed by certain actions, and amplifying that context representation increases those output probabilities

### Why Emotion-Shaped Representations Emerge

Emotion categories are a highly efficient compression scheme for predicting human text. Knowing the emotional context is more predictive of what comes next than surface-level features. The model converges on emotion-shaped representations not because it feels anything, but because Barrett's emotion categories turn out to be useful tools for text prediction too. Same tool, different substrate, different purpose.

The post-training finding confirms this: RLHF reshaped the model's "emotional profile" to match what raters rewarded. The model's emotional representations aren't its own — they're a mirror of training preferences.

### Implication for Abby

If Abby should have something genuinely analogous to emotions — not reflections of human emotional text — it needs:
- A non-linguistic substrate for affect (core affect independent of language)
- Embodied consequences (internal states that change how the system processes everything)
- Emotions emerging from the system's own experience, not from imitating human expression patterns

See also: [[inherited-tools]] [[intelligence]] [[brain]] [[grokking]] [[unconstrained-thought]]
