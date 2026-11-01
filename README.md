<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1b27,55:24283b,100:3d59a1&height=190&section=header&text=Amar%20Tiwari&fontSize=54&fontColor=ffffff&fontAlignY=38&desc=AI%20Engineer%20%C2%B7%20Voice%20AI%20%C2%B7%20Agentic%20Systems%20%C2%B7%20RAG&descSize=17&descAlignY=60&descColor=a9b1d6" width="100%" alt="Amar Tiwari, AI Engineer" />
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=19&pause=1400&color=70A5FD&center=true&vCenter=true&width=620&lines=Voice+agents+that+answer+real+phone+calls;Agentic+pipelines+with+Claude%2C+LangGraph+and+MCP;RAG+that+keeps+working+with+no+internet;Architecture+%E2%86%92+evals+%E2%86%92+deployment" alt="Typing intro" />
</div>

<br/>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0yMC40NSAyMC40NWgtMy41NXYtNS41N2MwLTEuMzMtLjAzLTMuMDQtMS44NS0zLjA0LTEuODUgMC0yLjE0IDEuNDUtMi4xNCAyLjk0djUuNjdIOS4zNVY5aDMuNDF2MS41NmguMDVjLjQ4LS45IDEuNjQtMS44NSAzLjM3LTEuODUgMy42IDAgNC4yNyAyLjM3IDQuMjcgNS40NnY2LjI4ek01LjM0IDcuNDNhMi4wNiAyLjA2IDAgMSAxIDAtNC4xMiAyLjA2IDIuMDYgMCAwIDEgMCA0LjEyek03LjEyIDIwLjQ1SDMuNTZWOWgzLjU2djExLjQ1eiIvPjwvc3ZnPg==)](https://www.linkedin.com/in/amar-tiwari26)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:amar.tiwari.8355@gmail.com)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Tiwari__Amar)
[![Resume](https://img.shields.io/badge/Resume-3D59A1?style=for-the-badge&logo=readdotcv&logoColor=white)](./Amar_Tiwari_Resume.pdf)
[![Cortex live demo](https://img.shields.io/badge/Live_Demo-Cortex-1a1b27?style=for-the-badge&logo=vercel&logoColor=white)](https://cortex-sre.vercel.app)

</div>

---

## About

I'm an AI Engineer at **Communication Crafts** in Ahmedabad. I build LLM systems that real users depend on: voice agents that answer actual phone calls, agentic pipelines that do a sales team's research, and RAG platforms that keep working on a ship with no internet.

I own the whole lifecycle, not just the model call: system design, third-party and MCP integrations, tracing, evals, guardrails and deployment.

```text
Building   →   Voice AI · Agentic AI · RAG · LLM integrations
Stack      →   Python · FastAPI · LangGraph · MCP · Qdrant · Pipecat · Docker
Open to    →   AI Engineer roles · remote (worldwide) or Ahmedabad
```

---

## Featured Work

### 🎙️ Voicely: Voice AI Agents for Indian Telephony

> **No-code voice agents that make and answer real phone calls, in Hindi, Hinglish and 10 more Indian languages.**

You design the conversation on a visual canvas as a graph of steps. On a live call, every connection between steps becomes an LLM function call, so the agent decides when to move on by understanding the caller, not by matching keywords.

```text
caller ⇄ Twilio / Exotel ⇄ STT → LLM agent (flow graph + tools) → TTS ⇄ caller
```

- Real-time **STT → LLM → TTS** pipeline on Pipecat with swappable providers (Sarvam, Deepgram, OpenAI, ElevenLabs), keeping 8 kHz telephony audio end to end
- During a call the agent can **call HTTP tools**, search a **multilingual knowledge base**, and afterwards **extract structured fields** to CSV
- Every call keeps a stereo recording and a timestamped transcript showing each step, tool call and search
- Safeguards: TRAI calling-hours enforcement, Twilio signature verification, recovery when a provider fails mid-call, and a carrier simulator to test latency without a phone

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Pipecat](https://img.shields.io/badge/Pipecat-24283b?style=flat-square)
![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=flat-square&logo=webrtc&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=flat-square)
![Exotel](https://img.shields.io/badge/Exotel-1F6FEB?style=flat-square)
![Deepgram](https://img.shields.io/badge/Deepgram-13EF93?style=flat-square&logo=deepgram&logoColor=black)
![ElevenLabs](https://img.shields.io/badge/ElevenLabs-000000?style=flat-square&logo=elevenlabs&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Status](https://img.shields.io/badge/Company_product-private-555?style=flat-square)

---

### 🤖 AI Lead Generation System

> **Finds companies that need our services, researches them with Claude and drafts the first outreach. Built solo.**

It started as my **2nd-place prototype** at an internal Agentic AI Hackathon. I then built it into the production system the sales team uses, and the client feedback has been strong.

```text
10+ sources → keyword match → Claude research → ICP score /100 → decision maker → drafts → rep review
```

- A scraper agent collects job and project posts from **10+ sources** (public APIs, RSS, JSON-LD, headless browser, IMAP email alerts, Upwork GraphQL) and matches them against 245 service keywords
- It doesn't fight the sites it reads: robots.txt is enforced in code, there's no stealth or CAPTCHA solving, and a source that blocks it pauses itself
- **Claude research agents** check each company (Apollo + web), score it on a **100-point ICP model with cited evidence**, find the decision maker, and draft an email and LinkedIn note for a rep to approve
- A React dashboard traces every search, page, token and dollar per step, shows **cost per sales-ready lead**, and has dry-run, controlled and full run modes

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=claude&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white)
![Status](https://img.shields.io/badge/Company_product-private-555?style=flat-square)

---

### 🚢 MarineDoc: Offline-First Multi-Tenant RAG

> **Ship crews ask questions about their technical manuals and get cited, page-level answers, even in the middle of the ocean.**

Built in **one month with a team of two**, and awarded a **WOW Card** at Communication Crafts. Ships often have no internet, so the system works in three modes:

| Mode | When | What happens |
|------|------|--------------|
| **Online** | Internet available | LLM answer streamed with citations (Groq · Llama 3.1, SSE) |
| **Intranet** | Ship server reachable, no internet | Ranked manual passages from the server's hybrid retrieval, no LLM call |
| **Offline** | No server at all | The phone runs its own retrieval with ONNX embeddings + sqlite-vec |

- **Hybrid retrieval:** per-tenant BM25 + dense search (Qdrant), RRF fusion, two-stage cross-encoder reranking and parent-child chunk expansion
- **PDF ingestion that adapts to the file:** a fast PyMuPDF path handles a 50-page manual in 1–3 s, and only scanned or messy pages fall back to YOLOX layout analysis and Tesseract OCR
- **Full SaaS:** tenant isolation, two-level RBAC (who can call which API, who can see which document), plans and quotas, a super-admin console and audit log
- **React Native app** with delta sync filtered by each user's access, and request-level trace IDs on every log line

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX_Runtime-005CED?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
[![Repo](https://img.shields.io/badge/Repo-hybrid--rag--chatbot-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Amar5623/hybrid-rag-chatbot)

---

## More Projects

| Project | What it does | Built with |
|---|---|---|
| [**Cortex**](https://github.com/Amar5623/cortex) · [demo](https://cortex-sre.vercel.app) | A 6-agent SRE incident-response swarm across 2 AWS regions. CockroachDB is its only memory, so when one region is killed mid-fix, the other picks up where it left off | LangGraph · AWS Lambda · CockroachDB · MCP |
| [**PipelineGuard**](https://github.com/Amar5623/Pipeline-Guard) | Generates dbt and Airflow code from the real schema, lineage, PII tags and SLAs in DataHub, then writes lineage back | DataHub MCP · Gemini · Python |
| [**StandupPilot**](https://github.com/Amar5623/standup-pilot) | A Slack agent that runs async standups and checks reported blockers against live workspace conversations | Slack Bolt · Slack MCP · Groq |
| [**EZ-Insights**](https://github.com/Amar5623/ez-insights) | Natural language to SQL with self-correcting retries, a 15-category SQL-injection validator and sensitive-column filtering | FastAPI · FAISS · Pinecone · Next.js |
| [**Customer Support Agent**](https://github.com/Amar5623/customer-support-agent) | A 2-tier meta-tool design that keeps tool schemas at about 750 tokens per request, plus human-in-the-loop approvals | FastAPI · Groq · MongoDB · WebSockets |

---

## How I Build

| | |
|---|---|
| 🏗️ **Architecture** | Multi-tenant isolation, offline-first sync, multi-agent workflows with parallel steps, conversation graphs compiled into function calls |
| 🔌 **Integrations** | REST and GraphQL APIs, webhooks, WebSockets, WebRTC, and MCP servers (DataHub, Slack, CockroachDB) |
| 🔍 **Tracing & monitoring** | Request trace IDs, token and cost tracing per step, call transcripts with tool events, audit logs |
| 🧪 **Evals & guardrails** | Latency simulators, staged rollouts (dry run → controlled → full), PII reports, SQL-injection validation, least-privilege agent roles |
| 🚀 **Deployment** | Docker, AWS Lambda + SAM across 2 regions, Railway, Render, Vercel, EAS builds for mobile |

---

## Tech Stack

**AI & LLMs**

![LangChain](https://img.shields.io/badge/LangChain-1a1b27?style=for-the-badge&logo=langchain&logoColor=70A5FD)
![LangGraph](https://img.shields.io/badge/LangGraph-1a1b27?style=for-the-badge&logo=langgraph&logoColor=70A5FD)
![LangSmith](https://img.shields.io/badge/LangSmith-1a1b27?style=for-the-badge&logo=langchain&logoColor=70A5FD)
![MCP](https://img.shields.io/badge/MCP-1a1b27?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-1a1b27?style=for-the-badge&logo=claude&logoColor=D97757)
![Gemini](https://img.shields.io/badge/Gemini-1a1b27?style=for-the-badge&logo=googlegemini&logoColor=8E75B2)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-1a1b27?style=for-the-badge&logo=huggingface&logoColor=FFD21E)
![Ollama](https://img.shields.io/badge/Ollama-1a1b27?style=for-the-badge&logo=ollama&logoColor=white)

**Vector Search & Voice**

![Qdrant](https://img.shields.io/badge/Qdrant-1a1b27?style=for-the-badge&logo=qdrant&logoColor=DC244C)
![FAISS](https://img.shields.io/badge/FAISS-1a1b27?style=for-the-badge&logo=meta&logoColor=0467DF)
![Pinecone](https://img.shields.io/badge/Pinecone-1a1b27?style=for-the-badge)
![Deepgram](https://img.shields.io/badge/Deepgram-1a1b27?style=for-the-badge&logo=deepgram&logoColor=13EF93)
![ElevenLabs](https://img.shields.io/badge/ElevenLabs-1a1b27?style=for-the-badge&logo=elevenlabs&logoColor=white)
![WebRTC](https://img.shields.io/badge/WebRTC-1a1b27?style=for-the-badge&logo=webrtc&logoColor=white)

**Languages, Backend, Frontend & Cloud**

<p>
  <img src="https://skillicons.dev/icons?i=python,ts,js,fastapi,postgres,mongodb,supabase,sqlite&theme=dark" alt="Python, TypeScript, JavaScript, FastAPI, PostgreSQL, MongoDB, Supabase, SQLite" />
  <br/>
  <img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,docker,aws,vercel,linux,git&theme=dark" alt="React, Next.js, Node.js, Docker, AWS, Vercel, Linux, Git" />
</p>

---

## Recognition

- 🥈 **2nd Place**, internal Agentic AI Hackathon, Communication Crafts (2026): built the lead-generation prototype that later went to production
- 🏅 **WOW Card** as an intern, for shipping MarineDoc in one month with a team of two
- 💰 **Bounty Winner**, [Level Up Your Aptos NFT Marketplace dApp](https://github.com/Amar5623/Aptos-NFT-Marketplace-Bounty)

---

## GitHub Activity

<div align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Amar5623&theme=tokyonight" width="100%" alt="GitHub contributions over the last year" />
</div>

<br/>

<div align="center">

*Open to AI Engineer roles, remote or in Ahmedabad. The fastest way to reach me is [email](mailto:amar.tiwari.8355@gmail.com).*

</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:3d59a1,45:24283b,100:1a1b27&height=100&section=footer" width="100%" alt="" />
</div>
