<<<<<<< HEAD
<p align="center">
  <img src="./assets/hero.svg" width="100%" alt="Amar Tiwari, AI Engineer: voice AI, agents and RAG. Open to AI engineering roles, remote or Ahmedabad." />
</p>

<p align="center">
  <a href="mailto:amar.tiwari.8355@gmail.com"><img src="https://img.shields.io/badge/Email-0F1522?style=for-the-badge&logo=gmail&logoColor=FFB547" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/amar-tiwari26"><img src="https://img.shields.io/badge/LinkedIn-0F1522?style=for-the-badge&logo=linkedin&logoColor=5B8CFF" alt="LinkedIn" /></a>
  <a href="https://x.com/Tiwari__Amar"><img src="https://img.shields.io/badge/X-0F1522?style=for-the-badge&logo=x&logoColor=EEF2F8" alt="X" /></a>
  <a href="https://cortex-sre.vercel.app"><img src="https://img.shields.io/badge/Live_demo-Cortex-0F1522?style=for-the-badge&logo=vercel&logoColor=34D399&labelColor=0F1522" alt="Live demo: Cortex" /></a>
</p>

```yaml
role:     AI Engineer @ Communication Crafts · Ahmedabad, India (IST)
builds:   voice agents on live phone lines · agentic pipelines · production RAG
owns:     architecture → integrations → tracing → evals → deployment
open_to:  AI engineering roles · remote (worldwide) or Ahmedabad
```

## Systems I've shipped

<img src="./assets/voicely.svg" width="100%" alt="Voicely: caller to carrier to speech-to-text to LLM agent to text-to-speech, with knowledge base, HTTP tools and post-call extraction" />

- **The conversation is a graph.** Each edge on the visual canvas compiles into an LLM function call, so the agent moves between stages by reasoning about what the caller said, not by matching keywords.
- **Built for real phone lines.** Audio stays at 8 kHz end to end, providers can be swapped at every step, and the agent can call HTTP tools, search a multilingual knowledge base and fill structured fields after the call.
- **Production safeguards:** TRAI calling-hours enforcement, Twilio signature checks, and fallback when a provider fails mid-call. A carrier simulator replays the real Twilio and Exotel protocols so latency can be tested without a phone.

<sub>Private company product · walkthrough available on request</sub>

<br/>

<img src="./assets/leadgen.svg" width="100%" alt="AI lead generation: sources to keyword match to Claude research agent to ICP score to decision maker to drafts for a sales rep" />

- **Respects the sites it reads.** robots.txt is enforced in code, there are no stealth or CAPTCHA workarounds, and sources that block it pause themselves.
- **Claude research agents** look into each company (Apollo + web), score it on a 100-point ICP model with cited evidence, and draft an email and LinkedIn note for a rep to review.
- **Every step is traced:** each search, page, token and dollar, plus cost per sales-ready lead, with dry-run, controlled and full run modes. It started as my **2nd-place** internal Agentic AI Hackathon prototype, and I built it into production on my own.

<sub>Private company product · walkthrough available on request</sub>

<br/>

<img src="./assets/marinedoc.svg" width="100%" alt="MarineDoc: query through hybrid retrieval (BM25 and dense, RRF fusion, reranking) to three modes: online, intranet and fully offline on the phone" />

- **Hybrid retrieval:** per-tenant BM25 + dense search in Qdrant, fused with RRF, then two-stage cross-encoder reranking and parent-child chunk expansion.
- **PDF ingestion that adapts to the file:** a fast PyMuPDF path handles a 50-page manual in 1–3 s, and only scanned or messy pages go through YOLOX layout analysis and Tesseract OCR.
- **A full SaaS around it:** tenant isolation, two-level RBAC, plans and quotas, a super-admin console with an audit log, and RBAC-scoped delta sync to a React Native app that runs the whole pipeline on the phone.

<sub>Built in one month with a 2-person team · earned a WOW Card · <a href="https://github.com/Amar5623/hybrid-rag-chatbot">repo</a></sub>

## How I engineer

| | What it looks like in my work |
|---|---|
| **Architecture** | Multi-tenant isolation and 3 connectivity modes (MarineDoc), conversation graphs compiled to function calls (Voicely), a 6-agent DAG with parallel fan-out (Cortex) |
| **Integrations** | Twilio, Exotel, Sarvam, Deepgram, ElevenLabs, Apollo, Supabase, Upwork GraphQL, IMAP, plus the DataHub, Slack and CockroachDB MCP servers |
| **Tracing & monitoring** | Per-request trace IDs, token and cost tracing at each step, call transcripts with node and tool events, append-only audit logs |
| **Evaluation** | A carrier simulator for latency testing, dry-run → controlled → full rollout gates, PII safety reports on generated code, feedback and outcome analytics |
| **Guardrails** | A 15-category SQL-injection validator, sensitive-column filtering, least-privilege SQL roles for each agent, separate read-only and write MCP sessions |
| **Deployment** | Docker, AWS Lambda in 2 regions with SAM, Railway, Render, Vercel, EAS builds for Android |

## More builds

| Project | What it shows | Links |
|---|---|---|
| **Cortex** | A 6-agent LangGraph SRE swarm across 2 AWS regions. CockroachDB is its only memory: lease locks and fenced writes let it survive a region being killed mid-fix | [repo](https://github.com/Amar5623/cortex) · [live](https://cortex-sre.vercel.app) · [video](https://youtu.be/34qlBkwNzJU) |
| **PipelineGuard** | A DataHub MCP agent that writes dbt and Airflow code from real schema, lineage, PII tags and SLAs, then writes lineage back | [repo](https://github.com/Amar5623/Pipeline-Guard) |
| **StandupPilot** | A Slack agent that uses Slack MCP and the Real-Time Search API to check reported blockers against live conversations | [repo](https://github.com/Amar5623/standup-pilot) |
| **EZ-Insights** | NL-to-SQL with schema RAG, self-correcting retries and a 15-category SQL-injection validator for live production databases | [repo](https://github.com/Amar5623/ez-insights) |
| **Support Agent** | A 2-tier meta-tool design that keeps tool schemas at about 750 tokens per request, plus human-in-the-loop approvals over WebSockets | [repo](https://github.com/Amar5623/customer-support-agent) |

## Toolbox

<p>
  <img src="https://skillicons.dev/icons?i=python,fastapi,ts,react,nextjs,docker,aws,postgres,mongodb,supabase,sqlite,vercel,linux,git&theme=dark&perline=14" alt="Python, FastAPI, TypeScript, React, Next.js, Docker, AWS, PostgreSQL, MongoDB, Supabase, SQLite, Vercel, Linux, Git" />
</p>

**LLMs & agents** · LangGraph · LangChain · LangSmith · MCP · tool calling · evals · guardrails · Claude · OpenAI · Groq · Gemini<br/>
**Retrieval** · BM25 + dense (RRF) · cross-encoder reranking · hierarchical chunking · Qdrant · Pinecone · FAISS · sqlite-vec<br/>
**Voice** · Pipecat · Sarvam · Deepgram · ElevenLabs · Twilio · Exotel · WebRTC<br/>
**Mobile** · React Native (Expo) · ONNX Runtime on device

## Recognition

- 🥈 **2nd place**, internal Agentic AI Hackathon at Communication Crafts (2026)
- 🏅 **WOW Card** as an intern, for shipping MarineDoc in one month with a 2-person team
- 💰 **Bounty winner**, [Aptos NFT Marketplace dApp](https://github.com/Amar5623/Aptos-NFT-Marketplace-Bounty)

<br/>

<p align="center">
  <sub>Hiring for AI engineering, remote or in Ahmedabad? The quickest way to reach me is <a href="mailto:amar.tiwari.8355@gmail.com">email</a>.</sub>
</p>
=======
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:16213e&height=140&section=header&text=Amar%20Tiwari&fontSize=48&fontColor=ffffff&fontAlignY=55&desc=AI%20Engineer%20%E2%80%94%20RAG%20%7C%20LLM%20Integration%20%7C%20Agentic%20AI&descSize=16&descAlignY=78&descColor=a0aec0" />
</div>

<br/>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/amar-tiwari26)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:amar.tiwari.8355@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Amar5623)
[![Portfolio](https://img.shields.io/badge/MarineDoc-0F4C81?style=for-the-badge&logo=anchor&logoColor=white)](#-flagship-project--marinedoc)

</div>

---

## About

AI Engineer Intern building production-grade RAG systems, NL-to-SQL pipelines, and agentic AI applications. I work end-to-end — retrieval architecture, backend, and Docker deployment — not just model wrappers.

Currently interning at **Communications Crafts** and independently building **MarineDoc**, a B2B SaaS AI platform for the maritime industry.

```text
Focus areas   →   RAG Systems · LLM Integration · Agentic AI · Vector Search
Stack         →   Python · FastAPI · Qdrant · LangChain · React Native · Docker
Open to       →   AI Engineer roles (remote / global)
```

---

## Flagship Project — MarineDoc

> **AI-powered document intelligence for the maritime industry — works fully offline at sea.**

Ship engineers upload their technical PDF manuals once. Then they ask questions in plain English and get cited, page-level answers — from their own documents, with zero hallucination risk. The system runs in three connectivity modes:

| Mode | State | How it works |
|------|-------|-------------|
| Online | Full internet / port | Streams AI-generated answers via Groq + Llama 3.1 |
| Intranet | Ship's local server, no satellite | Returns ranked document chunks from local Qdrant |
| Offline | Fully air-gapped at sea | ONNX model runs directly on the phone — zero cloud |

**Technical highlights:**
- Hybrid retrieval: BM25 + dense vector search + Reciprocal Rank Fusion
- TinyBERT cross-encoder reranking + hierarchical parent-child chunking
- Multi-tenant: each shipping company gets physically isolated Qdrant collections + BM25 indexes
- Full SaaS: admin panel, super-admin portal, plan tiers, audit logging, delta sync
- React Native mobile app with on-device ONNX inference (expo + nitro-onnxruntime)
- Deployed via Docker Compose — entire backend in one command

[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)](https://reactnative.dev)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://docker.com)
[![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)](https://supabase.com)
![Status](https://img.shields.io/badge/Status-Pre--launch-orange?style=flat-square)

---

## Projects

### RAG Document Chatbot
> Hybrid retrieval pipeline with production-grade auth and deployment

- BM25 + dense vector search + RRF fusion with CrossEncoder reranking
- Hierarchical parent-child chunking — supports PDF, CSV, XLSX, TXT
- Provider-agnostic backend switchable via env vars · JWT auth · rolling LLM conversation summary
- Real-time SSE streaming · deployed end-to-end via Docker Compose

[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](.)
[![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)](.)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](.)
[![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)](.)

---

### EZ-Insights — NL-to-SQL Engine
> Natural language to SQL for non-technical users on live production databases

- Dual-chunk RAG schema retrieval: raw DESCRIBE output + business-enriched YAML context
- 3-attempt self-correction retry loop feeding DB error messages back to the LLM
- 15-category SQL injection validator + 55+ sensitive field filtering and result-level data scrubbing
- Multi-DB: MySQL · MongoDB · PostgreSQL

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](.)
[![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logo=meta&logoColor=white)](.)
[![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white)](.)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)](.)

---

### Customer Support AI Agent
> Agentic system with human-in-the-loop approval and real-time notifications

- 2-tier meta-tool architecture (tool_search + tool_invoke via sentence-transformer embeddings)
- Caps per-request tool schema tokens at ~750 regardless of registry size
- Zero-LLM conversation compressor retaining 3 verbatim turns + structured summaries of older history
- Human-in-the-loop admin approval with real-time WebSocket push notifications

[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](.)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)](.)
[![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white)](.)
[![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)](.)

---

## Tech Stack

**AI & GenAI**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Vector Databases & Search**

![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge&logo=qdrant&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logo=meta&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=for-the-badge&logo=pinecone&logoColor=white)

**Backend & APIs**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

**Frontend & Mobile**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white)

---

## GitHub Stats

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Amar5623&theme=tokyonight&hide_border=true" width="60%"/>

</div>

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Amar5623&theme=tokyo-night&hide_border=true&area=true" width="100%"/>

</div>

---

<div align="center">

*Building real systems. Shipping real products.*

</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:16213e,100:1a1a2e&height=80&section=footer"/>
</div>
>>>>>>> cd7f390cba38e9896d3e701e295aac1c7e4b2a6e
