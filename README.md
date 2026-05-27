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
