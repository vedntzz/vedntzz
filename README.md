<img src="./banner.svg?v=2" alt="Vedant Srivastava — AI Engineer. Guardrails for coding agents: models propose, plain code decides." width="100%">

**I make AI coding agents safe to trust on a real codebase.** Four years of production backends at Capgemini and NBME taught me where systems break; now I build the guardrails that stop LLMs from breaking them.

**Hiring for AI Engineer or Backend?** I'm open to roles in Bengaluru, Delhi NCR, Hyderabad, Pune or remote.<br>
[LinkedIn](https://www.linkedin.com/in/vedant-srivastava-ai/) · [vedant.apple@gmail.com](mailto:vedant.apple@gmail.com) · [npm](https://www.npmjs.com/package/@vedantzz/session)

## Proof

| | |
|---|---|
| **1st place** | Philly CodeFest 2025, Comcast Challenge. Presented the winning build to Comcast's CFO |
| **Top 3% of ~20,000** | Cerebral Valley × Anthropic hackathon, judged by the Claude Code team |
| **~2,900 tests** | across Knack and The Session, both built test-first |
| **Shipped on npm** | [`@vedantzz/session`](https://www.npmjs.com/package/@vedantzz/session) |
| **Published** | *LLMs and Transfer Learning*, IJRPR Vol 4 Issue 11, 2023 |

## What I've built

### [Knack](https://github.com/vedntzz/Knack): never argue the same PR twice
*Solo, 10 days, Meta Global AI Developer Hackathon*

Every team has argued the same review point twice. The decision lives in a merged PR thread no coding agent has read, so the agent ships the rejected approach again. Knack reads that history, turns each decision into an ast-grep rule, and blocks the agent at edit time, citing the PR where it was decided.

- **No model in the verdict.** One Meta model proposes rules, a second attacks them with held-out variants. The block is plain code: no model, no network, 17 ms.
- **Run on real repos.** apache/airflow and fastapi: 101 PRs → 107 decisions → 12 rules → 5 that block. A person confirms before anything blocks.
- **Every number is reproducible.** One script re-derives every claim in ~80 s and ends `PROOF: PASS`. ~1,900 tests, pyright clean.

`Python` `ast-grep` `Meta Muse models` `Baseten`

### [The Session](https://github.com/vedntzz/The-Session): what did that AI coding session actually cost?
A CLI on npm that records every AI coding session as an Ed25519-signed hash chain anyone can verify. Found that naively summing Claude Code transcripts **overcounts spend by ~80%** and fixed it by deduping on request ID. Gives median/p90 cost estimates for a class of work. **1,000+ tests.**

`TypeScript` `Node`

### [Poneglyph](https://github.com/vedntzz/Poneglyph): document intelligence that cites the pixel
Multi-agent pipeline that detects drift across document versions and grounds every citation to the exact spot on the source page. Hybrid retrieval, cross-encoder reranking, RAGAS evals. **Top 3% of ~20k.**

`Python` `LangChain`

### [SkillEdge Pro](https://github.com/vedntzz/skilledgePro): resume in, learning path out
Skill-gap scoring against a target role plus an LLM-built plan to close the gaps. **Won Philly CodeFest 2025.**

`FastAPI` `React` `spaCy`

<sub>Also: [Ohara](https://github.com/vedntzz/Ohara), retrieval that refuses unsupported answers via an NLI check · [rag-generator](https://github.com/vedntzz/rag-generator), pluggable RAG with ports & adapters</sub>

## Where I've worked

| | |
|---|---|
| **NBME** · Software Engineer · 2025–26 | Modernized legacy services to Java 21 / Spring Boot 3 (Struts → Spring, javax → jakarta). Built AWS serverless error-reporting pipelines on Lambda, EventBridge, DynamoDB and CDK |
| **Synergy Technofin** · AI Engineer, contract · 2024–25 | Shipped GenAI skill-mapping in an HRMS (benchmarked BERT, chose Claude). Built agentic document retrieval over Microsoft Graph |
| **Capgemini** · Software Engineer · 2022–24 | Sole engineer on an SAP client account, owning DB design, dashboards and client demos. Split a client out of a shared ~50 GB database onto its own |

## Stack

**AI:** Claude Agent SDK, LangChain, LangGraph, RAGAS, PyTorch, HuggingFace, LoRA/PEFT, FAISS, Pinecone<br>
**Backend:** Java, Spring Boot, Python, FastAPI, TypeScript, Node, PostgreSQL, Redis, MongoDB<br>
**Cloud:** AWS (Lambda, EventBridge, DynamoDB, S3, CDK), Terraform, Docker · AWS & GCP certified

<sub>Projects are named after One Piece islands. If you catch the references, we'll get along.</sub>
