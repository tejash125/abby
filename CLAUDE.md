# Abby — Artificial Baby

## What is this project?

Abby is a long-term research project exploring how a baby might think and learn, replicated in an artificial simulated environment. The project questions foundational assumptions about computation, cognition, and learning — from programming paradigms to analog computing, neuromorphic chips, and custom hardware.

**P0 target:** An online learning system that continuously learns, integrates memory, and can understand analog clocks, the concept of time, and draw pictures of telling time accurately.

## Repository purpose

This repo is a **research workspace and Obsidian vault**. It serves as:
- Knowledge organization and summarization of research findings
- Linking and cross-referencing papers, ideas, and concepts
- Small coding experiments and proofs of concept
- Progress tracking toward eventual project delivery

## Project structure

```
research/          # Research notes, paper summaries, and linked concepts
personal-notes/    # Personal thoughts, key insights, and reflections
experiments/       # Coding experiments and proofs of concept
assets/            # Images, diagrams, and other media referenced in notes
```

## Research workflow

1. **Research in Claude Code** — discuss, question, and explore ideas directly in conversation
2. **Save to repo** — when something is worth keeping, ask Claude to write it as a structured note into `research/`
3. **Summarize external content** — ask Claude to fetch and summarize webpages, then save to repo
4. **Drop media into `assets/`** — images, diagrams, screenshots go here and are referenced from notes
5. **Browse in Obsidian** — open this repo as a vault in Obsidian for visual browsing, graph view, and linking

## Conventions

- Keep everything minimal — no templates, placeholders, or boilerplate
- Only add what is necessary and serves a clear purpose
- Research notes use Markdown with YAML frontmatter for metadata (date, tags, sources)
- Use `[[wikilinks]]` or relative markdown links to connect related notes
- Experiment directories are self-contained with their own README explaining the hypothesis and findings
- Commits are infrequent (every several days) — used as research backups, not granular tracking
- Do not commit unless explicitly asked
- When summarizing papers or concepts, always include source links
- Images and media go in `assets/`, referenced with relative paths

## Research domains (non-exhaustive)

- Developmental cognition and learning theory
- Online/continual learning systems
- Memory formation and integration
- Analog and neuromorphic computing
- Visual reasoning and spatial understanding
- Alternative computation paradigms

## Core communication principle

**Explain everything from first principles.** If a term hasn't been introduced and explained in this conversation, don't use it. No jargon, no acronyms, no shorthand that bakes in assumptions. Every concept should be explainable to a kid. If it can't be, we don't understand it well enough yet.

This is not about dumbing things down — it's about intellectual honesty. Using unexplained terminology hides complexity behind labels and goes against the entire spirit of this project. The goal is to build understanding from the ground up, not to import other people's abstractions unchecked.

When introducing a new concept:
1. Explain what it does in plain language first
2. Only then give it a name if it needs one
3. Never stack unexplained terms — if explaining A requires B, explain B first
4. If you catch yourself using jargon, stop and unpack it

## AI assistant guidance

- This is a research project — prioritize exploration and understanding over production quality
- Be minimal and clean — no unnecessary files, comments, abstractions, or scaffolding
- When asked to summarize or organize research, preserve nuance and link to sources
- When saving a research note, use YAML frontmatter with date, tags, and sources
- `personal-notes/key-insights.md` is for short, punchy one-liners — the sharpest ideas, not explanations. Link to the relevant research note for details.
- Do not link research notes to `personal-notes/` files — they are separate spaces. Research notes link to other research notes only. Personal notes can reference research notes but not the other way around.
- Experiments should be minimal and focused on testing a single idea
- Question assumptions freely — the whole point is rethinking fundamentals
- Help connect ideas across different research threads when relevant
- Tech stack is intentionally undefined — suggest tools only when a specific need arises

## Skill routing

When a request matches one of these gstack skills, invoke it via the Skill tool. Tailored to this research vault's workflow, not a code-shipping pipeline.

- Fetch and summarize a webpage → invoke /browse
- Pull structured data from a page → invoke /scrape
- Brainstorm or pressure-test a research idea → invoke /office-hours
- Debug a failing experiment → invoke /investigate
- Review experiment code before keeping it → invoke /review
- Save working progress mid-session → invoke /context-save
- Resume where you left off → invoke /context-restore
- Record a durable project learning → invoke /learn
