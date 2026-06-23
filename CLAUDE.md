# CLAUDE.md — Brain in a Vault

## Project Overview

This is a digital garden built with [Quartz](https://quartz.jzhao.xyz/) and published via GitHub Pages at `omertzuk.github.io/brain-in-a-vault`. The garden is authored by Omer Tzuk — physicist, complex-systems researcher, and contemplative neuroscientist — and focuses on consciousness studies, predictive processing, active inference, neurophenomenology, and related frameworks.

This project was created using Quartz's Obsidian template (run with `npx quartz create --template obsidian`). That template enables Obsidian-flavored markdown features such as wikilinks, callouts, and folder-note conventions which this site leverages.

All content lives in the `brain-in-a-vault/` folder as Markdown files. The garden is organized as a nested folder structure (see below), and notes are written in the **evergreen note** style: atomic, concept-centered, and heavily interlinked via wikilinks (`[[Note Name]]`).

---

## Folder Structure

```
brain-in-a-vault/
├── index.md                          ← Welcome page
├── Brain in a Vault.md               ← About this garden
├── Omer Tzuk.md                      ← Author note
│
├── maps/                             ← Maps of Content (navigational hubs)
├── concepts/
│   ├── consciousness/
│   ├── predictive-processing/
│   ├── active-inference/
│   ├── neurophenomenology/
│   ├── 4e-cognition/
│   └── information-theory/
├── theories/
├── methods/
├── papers/
└── projects/
```

---

## Note Conventions

- **Evergreen notes**: Each note in `concepts/` and `theories/` should be atomic — one idea per note, named as a noun or short concept phrase. Notes grow and are revised over time rather than being written once and abandoned.
- **Paper notes** (`papers/`): One note per paper. Should include: citation, core argument, key claims, limitations, and wikilinks to relevant concepts and theories.
- **Map of Content notes** (`maps/`): Navigational index notes that organize and link clusters of concept notes. Not content themselves — they surface structure.
- **Project notes** (`projects/`): Living documents for active research. Messy is fine here.
- **Wikilinks**: Use `[[Note Name]]` liberally. The link graph is the primary organizational mechanism of this garden.
- **Frontmatter**: Every note should include at minimum a `title` field. Tags are used as a cross-cutting layer alongside folders.

### Frontmatter template
```yaml
---
title: Note Title
tags:
  - tag1
  - tag2
---
```

---

## Domain Knowledge

The garden's intellectual core spans the following areas. Claude should treat these as the primary conceptual vocabulary when helping draft, expand, or link notes.

**Predictive Processing & Active Inference**
Karl Friston's Free Energy Principle (FEP) and Active Inference framework. Key concepts: variational free energy, Markov blankets, generative models, precision weighting, prediction error minimization, REBUS model (Relaxed Beliefs Under Psychedelics).

**Consciousness Studies**
Hard problem of consciousness, phenomenal vs. access consciousness, Global Workspace Theory, Integrated Information Theory, higher-order theories, altered states of consciousness.

**Neurophenomenology**
Varela's methodological program for bridging first-person phenomenology and third-person neuroscience. Key figures: Varela, Lutz, Thompson, Berkovich-Ohana. Key methods: micro-phenomenological interviews (MPI), neurophenomenological bracket, A1/A2 phenomenological phases.

**4E Cognition**
Embodied, embedded, enacted, extended approaches to mind. Enactivism (Varela, Thompson, Maturana), extended mind thesis (Clark & Chalmers).

**Information Theory**
Shannon entropy, mutual information, KL divergence, integrated information. Used as a cross-domain mathematical language connecting physics, neuroscience, and consciousness.

**Terror Management Theory (TMT)**
Ernest Becker's existential psychology formalized by Greenberg, Pyszczynski & Solomon. Mortality salience, worldview defense, and their neural correlates. Relevant to belief dynamics and identity-laden cognition.

**Complex Systems**
Pattern formation, self-organization, nonlinear dynamics, phase transitions. Background framework from Omer's physics training — useful for cross-domain analogies and formal modeling.

---

## Authoring Tasks Claude Should Support

### 1. Writing Evergreen Notes
When asked to draft a concept note, produce a focused, atomic note that:
- Opens with a 1–2 sentence crystallization of the core idea
- Develops the idea with appropriate depth (not a survey — go deep on what matters)
- Links generously to related notes via `[[wikilinks]]`
- Ends with open questions or unresolved tensions where relevant
- Includes appropriate frontmatter

### 2. Writing Paper Notes
When asked to write a literature note for a paper, produce a note that includes:
- Full citation
- Core argument in 2–3 sentences
- Key claims or findings (in prose, not bullet lists unless essential)
- Methodological notes if relevant
- Critical assessment: limitations, tensions, open questions
- Links to relevant concept and theory notes

### 3. Expanding and Linking
When asked to expand an existing note or suggest links, identify conceptual connections across the folder structure and propose specific wikilinks with brief justification for each connection.

### 4. Building Agents and Scripts
Claude may be asked to write Python or shell scripts to support garden maintenance — for example, generating note stubs, checking for broken wikilinks, building link graphs, or automating frontmatter. Scripts should be well-commented and assume a Unix environment.

### 5. Maps of Content
When asked to build or update a MOC, produce a structured navigational note that groups related concept notes thematically and surfaces the key tensions and open questions within that cluster.

---

## Style Guidelines

- **Prose over lists**: Notes should read as connected prose, not bullet-point summaries, except where a list is genuinely the clearest format.
- **Depth over breadth**: Better to develop one idea fully than survey many superficially.
- **Epistemic honesty**: Distinguish between established consensus, active debate, and speculative ideas. Use hedges like "one interpretation is..." or "this remains contested" where appropriate.
- **Voice**: The garden is a thinking space, not a textbook. Notes can be exploratory, can hold open questions, and can show the seams of ongoing thought.
- **Mathematical formalism**: Where relevant (especially in active inference and information theory notes), include formal notation. Omer has a physics background and mathematical depth is welcome.

---

## Publishing

- Built with Quartz 5, published to GitHub Pages at `omertzuk.github.io/brain-in-a-vault`
- Configuration lives in `quartz.config.ts` (or `quartz.config.yaml` as present in this project)
- Quartz renders wikilinks, LaTeX (via KaTeX), Mermaid diagrams, callouts, and Obsidian-flavored Markdown
- Do not modify files outside `brain-in-a-vault/` unless explicitly asked

---

## Key People

- **Omer Tzuk** — author; physicist and contemplative neuroscientist at the Contemplative Neuroscience and Neurophenomenology Lab, University of Haifa (PI: Aviva Berkovich-Ohana)
- **Aviva Berkovich-Ohana** — PI and methodological reference point for neurophenomenology work
- **Karl Friston** — primary theoretical figure for active inference / FEP
- **Francisco Varela** — founder of neurophenomenology; key figure for enactivism

---

## Review request

Please review and be familiar with the repository files that describe the site's philosophy and architecture (for example: `docs/philosophy.md`). Familiarity with these documents will help when drafting, linking, or reorganizing content in the garden.
