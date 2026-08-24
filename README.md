# Vedant Srivastava

I build LLM agent systems and the developer tooling around them.

Right now that means a CLI that turns AI coding sessions into a signed, verifiable record of what was spent and what actually shipped — on npm, 1,000+ tests. Before that, four years writing production backends: Spring Boot services at Capgemini, event-driven serverless on AWS at NBME. MS Software Engineering, Drexel, 2026.

I care about systems that hold up under real load and real money — correctness enforced in the database, not the prompt.

Open to AI Engineer and Backend roles.

[LinkedIn](https://www.linkedin.com/in/vedant-srivastava-a4a65b180/) · [vedant.apple@gmail.com](mailto:vedant.apple@gmail.com)

---

## Selected work

### The Session — `@vedantzz/session`
[npm](https://www.npmjs.com/package/@vedantzz/session) · [source](https://github.com/vedntzz/The-Session)

A CLI that measures what AI coding actually costs and what it actually shipped. Every session is recorded as an append-only, signed chain — Ed25519 keypair, per-record hash and previous-hash, so a third party can verify a log with no access to the signing machine. Outcome detection with tiered confidence, USD cost from measured token counts (deduped by request ID — naive line-summing of Claude Code transcripts overcounts by ~80%), and `session estimate` giving median/p90 cost for a class of work once enough history exists.

**1,000+ tests. Published on npm, v0.3.1.** TypeScript, Node, JSONL store, git-ref sync.

### Poneglyph
[source](https://github.com/vedntzz/Poneglyph)

Multi-agent document intelligence — messy ingest, temporal drift detection across document versions, pixel-grounded citations back to the source page. Hybrid dense + sparse retrieval with cross-encoder reranking, evaluated with RAGAS.

**Top 3% of ~20,000 entrants, Cerebral Valley × Anthropic hackathon.** Python, LangChain, Vercel/Railway.

### SkillEdge Pro
[source](https://github.com/vedntzz/skilledgePro)

Multi-agent recruitment platform — skill-gap analysis, project-to-candidate matching, recruiter dashboards. LangGraph orchestration over LangChain, Node, PostgreSQL, Docker.

**1st place, Philly CodeFest 2025 (Comcast Challenge).**

### Ohara
[source](https://github.com/vedntzz/Ohara)

Retrieval engine for technical documentation. Hybrid dense + sparse search, cross-encoder reranking on the candidate set, and an NLI check that refuses to answer when the retrieved context doesn't entail the claim — so it returns nothing rather than something wrong. Scored with RAGAS. Python, LangChain, FAISS.

---

## Stack

**Languages** Java · Python · TypeScript · SQL
**Backend** Spring Boot · FastAPI · Node/Express
**AI** Claude Agent SDK · LangChain · LangGraph · PyTorch · HuggingFace · LoRA/PEFT · RAGAS · FAISS · Chroma · Pinecone
**Cloud** AWS Lambda · S3 · DynamoDB · EventBridge · CDK · Terraform · Docker · Railway
**Data** PostgreSQL · MongoDB · Redis · SQLite
**Frontend** React · Next.js · Angular

AWS Cloud Practitioner · GCP Cloud Digital Leader

---

<sub>Projects are named after One Piece islands. If you catch the references, we'll get along.</sub>
