---
date: 2026-04-13
tags: [brain, neuroscience, architecture, cognition, foundations]
sources:
  - "Kandel, Eric — Principles of Neural Science"
  - "Damasio, Antonio — Descartes' Error (1994)"
  - "O'Keefe & Moser — Place cells and grid cells (Nobel Prize 2014)"
  - "Gazzaniga, Michael — split-brain experiments"
---

# Brain

## Level 0: Three Major Divisions

Evolutionarily stacked from oldest to newest:

```
┌─────────────────────────────┐
│         CEREBRUM            │  ← newest, largest, "the thinking part"
│    (forebrain)              │
├─────────────────────────────┤
│        CEREBELLUM           │  ← "little brain" at the back
├─────────────────────────────┤
│        BRAINSTEM            │  ← oldest, connects to spinal cord
│  (midbrain + pons + medulla)│
└─────────────────────────────┘
```

---

## Level 1: Brainstem — Keeps You Alive

The oldest part. Shared with reptiles. Handles everything you don't think about.

- **Medulla oblongata** — breathing, heart rate, blood pressure, swallowing, vomiting. Damage = death.
- **Pons** — relays signals between cerebrum and cerebellum. Involved in sleep/wake cycles, breathing regulation.
- **Midbrain** — eye movement, auditory and visual reflexes ("something moved" → you turn before deciding to). Contains the **substantia nigra** (dopamine production; degeneration → Parkinson's).
- **Reticular formation** — diffuse network through the brainstem. Controls arousal and consciousness at the most basic level. Damage → coma. The "on/off switch" for awareness.

The brainstem is the OS kernel. Runs before anything else boots, and if it crashes, nothing else matters.

## Level 1: Cerebellum — Coordination and Prediction

Sits at the back, below the cerebrum. Contains **more than half of all neurons** (~69 billion out of ~86 billion) despite being ~10% of brain volume.

- **Motor coordination** — smooth, precise movement. Damage → ataxia (clumsy, can't touch your nose with eyes closed)
- **Timing** — precise temporal coordination of muscle sequences. Catching a ball, playing piano, speaking fluently
- **Motor learning** — "practice makes automatic." Riding a bike, typing, muscle memory
- **Prediction** — increasingly recognized as a general-purpose prediction engine. Builds internal models of what *should* happen and flags errors when reality differs

The cerebellum is a prediction-error machine: predicts sensory feedback from a motor command, compares to reality, adjusts the model. Close to predictive coding frameworks.

## Level 1: Cerebrum — Everything You Think Of As "Thinking"

The largest part. Two hemispheres connected by the **corpus callosum**. Two major zones:
- **Cortex** (outer wrinkly surface) — newest, most "human"
- **Subcortical structures** (deep inside) — older, handles emotion, memory, reward, drives

---

## Level 2: The Cortex — Four Lobes

A 2-3mm thick sheet of neurons, folded to increase surface area ~3x. Flattened out, roughly the size of a large pizza.

```
         ┌──────────────────┐
         │   FRONTAL LOBE   │  ← planning, decision, personality
         │                  │
         ├──────────────────┤
         │  PARIETAL LOBE   │  ← spatial, sensory integration
         ├─────────┬────────┤
         │TEMPORAL │OCCIPITAL│
         │  LOBE   │  LOBE   │
         │(sides)  │ (back)  │
         └─────────┴─────────┘
```

### Frontal Lobe — Executive Control

The largest lobe. What makes humans most distinctly human.

- **Prefrontal cortex (PFC)** — planning, decision-making, working memory, personality, social behavior, impulse control. The "CEO." Last to fully develop (~age 25). Damage → personality changes, poor judgment (Phineas Gage case).
  - **Dorsolateral PFC** — working memory, cognitive flexibility, planning
  - **Ventromedial PFC** — emotional decision-making, risk assessment. Where Damasio's somatic markers operate. Damage → logical reasoning intact but catastrophic life decisions
  - **Orbitofrontal cortex** — reward evaluation, social norms, impulse control
- **Motor cortex** — direct control of voluntary movement. Organized as a body map (homunculus). Hands and face get disproportionately large regions.
- **Premotor cortex** — planning and preparing movements before execution
- **Broca's area** — speech production. Damage → understands language but can't produce fluent speech (Broca's aphasia)

### Parietal Lobe — Spatial Processing and Integration

- **Somatosensory cortex** — touch, temperature, pain, proprioception. Also organized as a body map.
- **Posterior parietal cortex** — spatial awareness, attention, coordinate transformations. Damage → hemispatial neglect (ignores one entire half of space)
- **Angular gyrus** — integration of language, number processing, spatial cognition, memory retrieval. A multimodal convergence zone.

### Temporal Lobe — Hearing, Language, Recognition

- **Auditory cortex** — sound processing. Organized tonotopically (different regions for different frequencies).
- **Wernicke's area** — language comprehension. Damage → fluent but nonsensical speech.
- **Fusiform face area** — face recognition. Damage → prosopagnosia (can't recognize faces).
- **Inferior temporal cortex** — object recognition. The "what is it?" pathway.

### Occipital Lobe — Vision

- **Primary visual cortex (V1)** — first cortical processing of visual input. Organized retinotopically.
- **V2, V3, V4, V5/MT** — progressively more abstract visual processing:
  - V1: edges, orientations
  - V2: contours, figure-ground
  - V4: color, shape
  - V5/MT: motion
- Two output streams:
  - **Ventral stream** ("what pathway") → temporal lobe → object identification
  - **Dorsal stream** ("where/how pathway") → parietal lobe → spatial location, guiding action

---

## Level 2: Subcortical Structures — The Deep Brain

Evolutionarily older. Handles things too important or too fast for conscious deliberation.

### Thalamus — The Relay Station

Almost all sensory info passes through the thalamus before reaching cortex (exception: smell → goes directly, possibly why smells trigger memories so powerfully).

Not just passive relay — **filters and gates** information. Decides what gets forwarded and what gets suppressed. During sleep, blocks most sensory input. Why you sleep through constant noise but wake to your name.

Thalamocortical loops (thalamus ↔ cortex feedback cycles) are thought essential for conscious awareness. Damage → coma.

### Hypothalamus — The Body's Thermostat

Tiny (~4g, almond-sized) but controls homeostasis:
- Body temperature, hunger, thirst
- Sleep-wake cycles (circadian rhythm, via suprachiasmatic nucleus)
- Hormone regulation (controls pituitary gland → entire endocrine system)
- Sexual behavior, fight-or-flight activation

Bridge between nervous system and hormonal system. Translates neural signals into hormonal signals and vice versa. Key player in generating core affect (valence + arousal).

### Hippocampus — Memory Formation

Shaped like a seahorse. Critical for:
- **Forming new explicit memories** — damage → anterograde amnesia (patient H.M.)
- **Spatial navigation** — London taxi drivers have enlarged hippocampi
- **Memory consolidation** — transfers short-term to long-term during sleep via replay

Forms memories but doesn't store them long-term. Long-term memories are distributed across cortex. The hippocampus is the indexer, not the hard drive.

Substructures:
- **CA1, CA3** — different aspects of memory encoding
- **Dentate gyrus** — one of two regions with adult neurogenesis. Helps separate similar memories.
- **Place cells** — fire when you're in a specific location. A literal spatial map.
- **Grid cells** (adjacent entorhinal cortex) — hexagonal grid pattern during movement. A coordinate system. Nobel Prize 2014.

### Amygdala — Salience Detection

Not the "fear center" (outdated). More accurately: **salience detection and emotional significance tagging.**

- Evaluates stimuli: "is this important? should I pay attention?"
- Processes both threats AND rewards
- Modulates memory — emotional memories are stronger because amygdala signals hippocampus "remember this"
- Fast shortcut: gets sensory input from thalamus *before* cortex finishes processing. Why you flinch at a stick before identifying it as not-a-snake.

### Basal Ganglia — Action Selection and Habits

A group of deep nuclei:
- **Striatum (caudate + putamen)** — input station, receives from cortex
- **Globus pallidus** — output station, inhibitory signals to thalamus
- **Subthalamic nucleus** — modulates the system

Functions:
- **Action selection** — cortex proposes many actions simultaneously. Basal ganglia selects which one executes, suppresses the rest. A gate, not a generator.
- **Habit formation** — repeated behavior shifts from cortex (deliberate) to basal ganglia (automatic). Why habits feel effortless.
- **Reward learning** — works with dopamine. Reward prediction errors drive learning.

Damage → Parkinson's (can't initiate movement), Huntington's (uncontrolled movement).

---

## The Wiring Principle

These are not isolated modules. The brain is a **recurrent, massively parallel network**:
- Almost every region connects back to its inputs (feedback loops everywhere)
- Cortex and subcortical structures in constant dialogue
- Top-down signals (expectations, predictions) are as important as bottom-up signals (sensory data)
- The thalamocortical loop processes in cycles, not one direction

This architecture is fundamentally different from any artificial neural network. The brain's wiring IS its computation.

---

## Quick Reference: Activity → Brain Region

| What you're doing | Primary region(s) |
|---|---|
| Breathing, heartbeat, staying alive | Medulla oblongata |
| Sleeping / waking up | Pons, reticular formation, hypothalamus |
| Being conscious at all | Reticular formation, thalamocortical loops |
| Seeing something | Occipital lobe (V1 → V2 → V4/V5) |
| Hearing something | Temporal lobe (auditory cortex) |
| Feeling touch, pain, temperature | Parietal lobe (somatosensory cortex) |
| Recognizing a face | Temporal lobe (fusiform face area) |
| Recognizing an object | Temporal lobe (inferior temporal cortex) |
| Knowing where something is in space | Parietal lobe (posterior parietal cortex) |
| Understanding speech | Temporal lobe (Wernicke's area) |
| Producing speech | Frontal lobe (Broca's area) |
| Moving your body voluntarily | Frontal lobe (motor cortex) |
| Smooth, coordinated movement | Cerebellum |
| Learning a physical skill (bike, piano) | Cerebellum + basal ganglia |
| Planning what to do next | Frontal lobe (prefrontal cortex) |
| Holding info in mind temporarily | Dorsolateral prefrontal cortex |
| Making a decision with emotional weight | Ventromedial prefrontal cortex |
| Controlling impulses | Orbitofrontal cortex |
| Forming a new memory | Hippocampus |
| Recalling an old memory | Hippocampus (retrieval) + cortex (storage) |
| Navigating physical space | Hippocampus (place cells) + entorhinal cortex (grid cells) |
| "Is this important?" / salience detection | Amygdala |
| Emotional memory boost ("remember this!") | Amygdala → hippocampus |
| Reacting before thinking (flinch) | Amygdala (thalamic shortcut) |
| Habits and automatic behaviors | Basal ganglia |
| Choosing one action, suppressing others | Basal ganglia |
| Reward, motivation, "wanting" | Basal ganglia + dopamine (VTA, substantia nigra) |
| Hunger, thirst, body temperature | Hypothalamus |
| Hormone regulation | Hypothalamus → pituitary gland |
| Filtering what reaches awareness | Thalamus |
| Sense of unified self | Default mode network (distributed) |
| Predicting what happens next | Cerebellum + cortex (distributed) |

See also: [[energy-cost-of-intelligence]] [[consciousness-and-the-label-problem]] [[emotions-and-constructed-affect]] [[information_processing]]
