# Hugin

**AI application & agent engineering** — I build auditable LLM tooling for government and enterprise workflows. Background in GIS, digital twins, and toG delivery, which is where the domain rigor comes from.

> AI 应用 / Agent 工程 · 出身 GIS、数字孪生与政企交付,现在做能审计、能落地的 LLM 工具链。

### What I build

Not demos. Production-shaped tooling where the hard part is **verification, not generation** — pipelines an LLM runs but a human or a state machine stays in control of. Most of my work lives in the gap between "the model produced something" and "the output is trustworthy enough to hand to a government client."

How I work: eval/fixture-first, auditable pipelines where every output traces back to its inputs, and a hard rule that documentation matches runtime behavior — no claimed capability the code doesn't actually execute.

### Selected work

- **[agentic-kb-lite](https://github.com/Hugin-Z/agentic-kb-lite)** — Local knowledge base over `ripgrep` + an LLM agent loop. No vectors, no embedding service, no external API, multimodal. The bet: at personal/team corpus scale, grep + a reasoning loop beats a vector stack on cost, transparency, and maintenance. v0.4 adds a pluggable *recipe* layer for dirty-document preprocessing — parsing upstream, retrieval downstream, kept separate.
- **[tender-writer-v4](https://github.com/Hugin-Z/tender-writer-v4)** — A Python state-machine toolchain for Chinese government technical-bid (技术标) writing. It compresses the first-pass structural breakdown and draft assembly of a bid down to minutes; formal submission still needs human expansion, checking, and review. A 5-stage auditable workflow with the LLM as orchestrator and the user gating each stage.
- **[solution-drafter](https://github.com/Hugin-Z/solution-drafter)** — A Skill framework for Chinese gov/enterprise (toG/toB) proposal documents. Three-layer decoupling — L1 framework / L2 document-type / L3 domain plugin — over a 5-stage workflow. Every example in the repo is fictional sample data.
- **[几境 / Nine Realms](https://9jing.top)** — A bilingual site mapping *skill at using AI* onto a 9-tier xianxia cultivation ladder. Built to make a fuzzy question — what does "good at AI" even mean — concrete and testable.

Some of my stronger work is closed or client-deployed and isn't linkable here: a planning-compliance self-inspection tool in production use at a district planning bureau, and 疆理 — a Rust/Tauri desktop app for agricultural land-use optimization (NSGA-II/III + Entropy-TOPSIS on national soil-survey data).
