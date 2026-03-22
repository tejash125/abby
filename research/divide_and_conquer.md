---
date: 2026-02-22
tags: [problem-solving, systems-design, foundational]
sources: []
---

# Divide and Conquer

The fundamental tension: splitting a problem gains parallelism and manageability but loses cross-cutting context. This applies everywhere — AI agent pipelines, organizations, software architecture.

## When to Split a Problem

Split reluctantly, not eagerly. Split when the cost of holding everything in one context exceeds the cost of managing the seams between sub-problems.

Conditions that make splitting viable:
- **Natural fault lines** — parts that interact weakly with each other. If sub-problems share many signals, splitting is dangerous.
- **Parallelism buys enough** to offset coordination overhead. If sub-problems are sequential and interdependent, splitting creates more problems than it solves.
- **The whole is too large** for any single reasoner (human, team, or LLM context window) to hold coherently.

Common mistake: splitting for organizational convenience (team boundaries, tool limitations) rather than because the problem genuinely decomposes that way. Conway's Law — system architecture mirrors org structure, even when that's the wrong decomposition.

## How to Manage Information Loss Across Levels

### Pass anomalies, not summaries
Summaries compress away the signal. "Entity X scored 0.8 on fraud" loses the *why*. Passing structured anomalies ("X made 47 small transactions to new accounts in 3 hours after 2-week dormancy") lets higher levels reason about cross-domain patterns. The feature is more portable than the score.

### Flag what you can't explain
Sub-agents should surface cases where their model is uncertain or behavior is unusual even below threshold. Unexplained residuals are often where cross-domain patterns live.

### Build a shared representation layer
Instead of sub-agents passing results to a coordinator (lossy telephone), have them write to a shared entity profile that accumulates evidence across domains. The coordinator reads richer signal.

### Uncertainty must travel upward explicitly
If a sub-agent isn't sure, that uncertainty needs to be represented — not collapsed into a binary or a score. Coordinators making decisions on "confident sub-agent outputs" are systematically misled.

## The Systemic Solution

Context is a resource. Most systems don't manage it deliberately.

1. **Decompose along information structure, not convenience.** Map the dependency graph before splitting. Cut at the thinnest edges — sub-problems that share many inputs or feed each other's outputs are poor split candidates.

2. **Design the interface between levels first.** What decisions does the higher level make? What information is necessary and sufficient? Everything beyond that is noise.

3. **Run periodic full-context sweeps.** A high-context reasoner periodically looks at the whole problem without sub-agent framing. Expensive, but it's the error-correction mechanism. Without it, the system drifts toward local optima while missing global patterns.

The bureaucracy problem in large companies is a failure of #3 — full-context sweeps become politically costly (they expose redundancy, challenge team boundaries) so they stop happening, and the organization optimizes locally until something big breaks.

## Relevance to Abby

If Abby's architecture requires decomposition (specialized subsystems for vision, memory, time-reasoning), the interfaces between them matter more than the subsystems themselves. The cross-cutting patterns are where understanding lives. See [[emergence]].
