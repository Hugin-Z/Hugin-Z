# Hugin

**AI application & agent engineering** — I build tool-using agents for real-world decisions, grounded by external data, explicit state, evidence, and human-visible uncertainty.

> AI 应用 / Agent 工程。做能查真实数据、保留证据与不确定性、最后给出可执行结果的 Agent。

My background is in GIS, digital twins, and government / enterprise delivery. That makes me care less about how fluent an AI looks, and more about whether its output can be **traced, verified, and acted on**.

### What I build

The model is not the source of truth.

Train schedules come from railway data. Routes come from map services. Project claims come from source documents. Knowledge retrieval comes from the local corpus.

The model plans and reasons; **tools, contracts, and state decide what is trustworthy enough to become an answer.**

I tend to work eval/fixture-first, keep important state explicit, put gates around high-impact decisions, and make documentation match actual runtime behavior.

### Selected work

* **[trip-decider](https://github.com/Hugin-Z/trip-decider)** — An evidence-constrained travel planning agent. It verifies rail, local transit, prices, place identity, and return constraints before they enter an itinerary; unknown and conflicting facts remain visible instead of being silently filled by the model. Also usable as an itinerary verifier.

* **[Evidence Runtime](https://github.com/Hugin-Z/evidence-runtime)** — An evidence-constrained agent workflow for turning source materials into auditable deliverables: evidence readiness → constrained generation → Claim Audit → delivery gate. The writer can be an LLM or a human; unsupported content does not silently become a deliverable.

* **[agentic-kb-lite](https://github.com/Hugin-Z/agentic-kb-lite)** — A lightweight local knowledge base built around `ripgrep` + an LLM reasoning loop instead of a vector stack. Structure carries part of the retrieval semantics; fixtures keep agent behavior reproducible and inspectable.

* **[tender-writer-v4](https://github.com/Hugin-Z/tender-writer-v4)** — A state-machine workflow for Chinese government technical-bid writing. Five auditable stages, explicit human gates, and structured tracking from scoring requirements to draft assembly.

### Other experiments

* **[几境 / Nine Realms](https://9jing.top)** — A bilingual, nine-tier model for making the fuzzy idea of “being good at AI” more concrete and testable.

Earlier domain work includes client-deployed planning-compliance tooling and a Rust/Tauri desktop application for agricultural land-use optimization.

---

**Verification > generation.**
If an agent cannot tell what it knows, where it came from, and what still needs checking, I don't consider the workflow finished.
