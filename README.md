# Hugin

**AI application & agent engineering** — I build auditable LLM tooling for government and enterprise workflows. Background in GIS, digital twins, and toG delivery, which is where the domain rigor comes from.

> AI 应用 / Agent 工程 · 出身 GIS、数字孪生与政企交付,现在做能审计、能落地的 LLM 工具链。

### What I build

Not demos. Production-shaped tooling where the hard part is **verification, not generation** — pipelines an LLM runs but a human or a state machine stays in control of. Most of my work lives in the gap between "the model produced something" and "the output is trustworthy enough to hand to a government client."

How I work: eval/fixture-first, auditable pipelines where every output traces back to its inputs, and a hard rule that documentation matches runtime behavior — no claimed capability the code doesn't actually execute.

### Selected work

- **[agentic-kb-lite](https://github.com/Hugin-Z/agentic-kb-lite)** — Local knowledge base over `ripgrep` + an LLM agent loop. No vectors, no embedding service, no external API, multimodal. The bet: at personal/team corpus scale, grep + a reasoning loop beats a vector stack on cost, transparency, and maintenance.
- **[tender-writer-v3](https://github.com/Hugin-Z/tender-writer-v3)** — A Claude Skill for Chinese government tender (标书) writing: a 5-stage auditable workflow with scoring-matrix tracking. The value isn't drafting — it's compliance auditing and gap detection against the tender requirements.
- **[几境 / Nine Realms](https://9jing.top)** — A bilingual site mapping *skill at using AI* onto a 9-tier xianxia cultivation ladder. Built to make a fuzzy question — what does "good at AI" even mean — concrete and testable.

<!-- Add this line ONLY after the repo is actually public, otherwise it links to nothing: -->
<!-- - **solution-drafter** — A generalized toG/toB proposal-generation Skill: S1–S4 pipeline, font-policy contracts, end-to-end asset-acquisition chain. -->

Some of my stronger work is closed or client-deployed and isn't linkable here: a Python state-machine bid-document toolchain (tender-writer V4), a planning-compliance self-inspection tool in production use at a district planning bureau, and 疆理 — a Rust/Tauri desktop app for agricultural land-use optimization (NSGA-II/III + Entropy-TOPSIS on national soil-survey data).
