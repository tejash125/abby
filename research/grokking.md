---
date: 2026-03-23
tags: [learning, generalization, neural-networks, deep-learning, online-learning]
sources:
  - "Grokking: Generalization Beyond Overfitting on Small Algorithmic Datasets — Power et al. (2022), OpenAI"
  - "Neel Nanda mechanistic interpretability on grokking (Fourier features)"
  - https://youtu.be/D8GOeCFFby4?si=Zdgg5JmRemZnniPj
---

# Grokking

## What it is

A phenomenon where a neural network, long after memorizing the training set, suddenly generalizes — validation accuracy jumps sharply to near 100% with no gradual warning. Discovered by Power et al. (2022) at OpenAI.

## The Experiment

Small transformers trained on **modular arithmetic**: given `a` and `b`, compute `(a + b) mod p` for a prime `p`. Dataset is small and finite. ~30-50% used for training.

**What happens:**
1. Model quickly reaches ~100% training accuracy — pure memorization
2. Validation accuracy stays near chance — classic overfitting
3. Training continues far beyond this point
4. At some point, validation accuracy **suddenly snaps to ~100%**

The jump is abrupt, not gradual. The model appeared stuck, then grokked.

## Why It Happens — Mechanistic View

Neel Nanda probed the internals of grokked models and found they use **Fourier features** — the network's internal computation mirrors the periodic structure of modular arithmetic. The memorizing solution and the generalizing solution are **qualitatively different circuits**.

The model doesn't get incrementally better at the same strategy. It discovers a fundamentally different internal representation.

## The Weight Decay Mechanism ("Second Gradient Descent")

After memorization, training loss is near zero — no obvious gradient signal. But weight decay (L2 regularization) keeps applying pressure:

- The memorization solution is expensive: large weights needed to store specific examples
- The generalizing solution is cheaper: a compact algorithm needs smaller weights
- Weight decay slowly makes the memorizing solution unaffordable
- The network reorganizes toward the more efficient, generalizing circuit

It's not literally a second optimizer run — same SGD throughout — but weight decay becomes the dominant force once memorization is complete, effectively running a second optimization pass favoring compression over lookup.

## Does It Always Happen?

No. Conditions required:
- **Weight decay** — near-essential; without it models tend to stay memorized
- **Small, structured dataset** — clean algorithmic tasks, not messy real-world data
- **Extended training** — must train well past overfitting
- **Task with learnable underlying structure** — something compressible exists to find

Large-scale LLM pretraining doesn't exhibit clean grokking — the dynamics are different at scale and with noisy data.

## The Deeper Question: Finding Structure vs. Understanding Structure

Grokking shows the model converges to an internal representation that **structurally mirrors** the algorithm — not a lookup table. That is a real and meaningful finding.

But it is not the same as understanding the concept.

**What the model can do after grokking:**
- Produce correct outputs on unseen examples within the task

**What it cannot do:**
- Explain why the algorithm works
- Transfer the concept to a new context or notation
- Recognize modular arithmetic when it appears differently
- Know when the operation is the wrong tool

**What humans have that the model doesn't:** Semantic grounding. When a human learns addition, they get the mechanic (combining quantities), the rule stated explicitly, and examples that confirm it. The grokked model gets only examples and derives structure from them — from the outside in, not the inside out.

The model found the **syntax** of the algorithm. It does not have the **semantics**.

## The Richness Gap

One way to frame the difference: human conceptual understanding is a *web* — addition connects to counting, subtraction, geometry, physical intuition about quantity. The grokked model has one isolated slice of the concept with no connections. The difference may not be one of *kind* but of *richness and connectivity*.

## Relevance to Abby

Grokking raises a core design question: should Abby be given mechanics explicitly (conceptual instruction) and grounded with examples? Or should it derive structure from experience alone?

Pure-example learning *can* converge to structure — but it is slow, fragile, and narrow. The human developmental path combines both: concepts are partially transmitted (language, instruction) and partially derived (experience, play, exploration).

The gap between finding structure and understanding structure is exactly the gap between behavioral generalization and genuine comprehension. This is unsolved.

See also: [[intelligence]] [[numbers]] [[brain]]
