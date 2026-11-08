# Vedant Srivastava

**AI Engineer. I build guardrails for coding agents — models propose, plain code decides.**

4 years shipping production backends — Spring Boot at Capgemini, event-driven AWS serverless at NBME. MS Software Engineering, Drexel '26. My last two projects carry ~2,900 tests between them, and every headline number below has a command that reproduces it.

**Open to AI Engineer and Backend roles — Bengaluru, Delhi NCR, Hyderabad, Pune, or remote.** Relocating from Philadelphia.

[LinkedIn](https://www.linkedin.com/in/vedant-srivastava-ai/) · [vedant.apple@gmail.com](mailto:vedant.apple@gmail.com)

---

## Selected work

### Knack — never argue the same PR twice
[source](https://github.com/vedntzz/Knack) · built solo in 10 days, Meta Global AI Developer Hackathon

Your team already argued out how the code should look — in merged PR threads no coding agent has read. Knack reads that history, compiles each decision into an ast-grep rule, and blocks the agent at edit time when it ships the rejected alternative, citing who decided.

- **Two models, zero models in the verdict.** Muse Spark proposes rules; Muse Spark Open attacks them with held-out variants Spark never sees. The block itself is a plain-code hook: no model, no network, **17 ms**.
- **Tested on real repos.** apache/airflow + fastapi: 101 PRs → 107 decisions → 12 installed rules → 5 that block. A person confirms before anything can block.
- **Provable.** `scripts/reproduce.sh` re-derives every claim in ~80 s and ends `PROOF: PASS`. ~1,900 tests, pyright clean, receipts in a hash chain.

Python · ast-grep · uv · Meta Muse models · Baseten

### The Session — [`@vedantzz/session`](https://www.npmjs.com/package/@vedantzz/session)
[source](https://github.com/vedntzz/The-Session) · on npm

A CLI that measures what AI coding actually costs and what it actually shipped. Every session is an append-only, Ed25519-signed hash chain a third party can verify without the signing machine. Found that naive summing of Claude Code transcripts **overcounts cost by ~80%** — fixed by deduping on request ID. `session estimate` gives median/p90 cost for a class of work.

**1,000+ tests.** TypeScript · Node · JSONL · git-ref sync

### Poneglyph
[source](https://github.com/vedntzz/Poneglyph) · **Top 3% of ~20,000, Cerebral Valley × Anthropic hackathon**

Multi-agent document intelligence: temporal drift detection across document versions and pixel-grounded citations back to the source page. Hybrid dense + sparse retrieval, cross-encoder reranking, evaluated with RAGAS.

Python · LangChain · Vercel/Railway

### SkillEdge Pro
[source](https://github.com/vedntzz/skilledgePro) · **1st place, Philly CodeFest 2025 (Comcast Challenge)**

Resume + target role in, skill gaps and an LLM-built learning path out. spaCy parsing, gap scoring, OpenAI. FastAPI · React · SQLAlchemy

**Also:** [Ohara](https://github.com/vedntzz/Ohara) — doc retrieval with an NLI check that refuses unsupported answers · [rag-generator](https://github.com/vedntzz/rag-generator) — runtime-pluggable RAG, ports & adapters, strict TDD

---

## Stack

**Languages** Java · Python · TypeScript · SQL<br>
**Backend** Spring Boot · FastAPI · Node/Express<br>
**AI** Claude Agent SDK · LangChain · LangGraph · PyTorch · HuggingFace · LoRA/PEFT · RAGAS · FAISS · Pinecone<br>
**Cloud** AWS Lambda · S3 · DynamoDB · EventBridge · CDK · Terraform · Docker<br>
**Data** PostgreSQL · MongoDB · Redis · SQLite<br>
**Frontend** React · Next.js · Angular

AWS Cloud Practitioner · GCP Cloud Digital Leader

---

<sub>Projects are named after One Piece islands. If you catch the references, we'll get along.</sub>
