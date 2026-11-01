## Amar Tiwari

AI Engineer in Ahmedabad, India. I build LLM systems that run in production: voice agents on live phone lines, agentic research pipelines, and RAG that keeps working without internet.

I handle the whole lifecycle: architecture, integrations, tracing, evals and deployment.

Open to AI engineering roles, remote or in Ahmedabad. [Email](mailto:amar.tiwari.8355@gmail.com) · [LinkedIn](https://www.linkedin.com/in/amar-tiwari26) · [X](https://x.com/Tiwari__Amar)

### What I've shipped

**Voicely**: voice AI agents that make and answer real phone calls over Twilio and Exotel, in Hindi, Hinglish and 10 more Indian languages. Conversations are node graphs where every transition is an LLM function call, running on a real-time STT → LLM → TTS pipeline at 8 kHz.
<sub>Company product, private repo</sub>

**AI Lead Generation**: collects job posts from 10+ sources, then Claude agents research each company, score it on a 100-point ICP model and draft outreach for a sales rep to review. Every step is traced for tokens and cost. I built it alone, starting from my 2nd-place hackathon prototype.
<sub>Company product, private repo</sub>

**MarineDoc**: multi-tenant RAG over ship manuals with page-level citations. Hybrid retrieval (BM25 + Qdrant, RRF, cross-encoder reranking), plus a React Native app that runs the whole pipeline on the phone when the ship has no internet. Built in a month by a team of two.
<sub>[repo](https://github.com/Amar5623/hybrid-rag-chatbot)</sub>

### Other projects

- [**Cortex**](https://github.com/Amar5623/cortex): a 6-agent LangGraph swarm across 2 AWS regions that survives a region going down mid-task · [live demo](https://cortex-sre.vercel.app)
- [**PipelineGuard**](https://github.com/Amar5623/Pipeline-Guard): an agent that uses the DataHub MCP server to generate dbt and Airflow code from real schema, lineage and PII tags
- [**StandupPilot**](https://github.com/Amar5623/standup-pilot): a Slack agent that checks reported blockers against live workspace conversations
- [**EZ-Insights**](https://github.com/Amar5623/ez-insights): natural language to SQL with self-correcting retries and SQL-injection guardrails
- [**Customer Support Agent**](https://github.com/Amar5623/customer-support-agent): tool calling that stays at about 750 tokens of tool schemas per request, whatever the number of tools

### Stack

Python, TypeScript, FastAPI · LangGraph, LangChain, LangSmith, MCP · Qdrant, Pinecone, FAISS, PostgreSQL, Supabase, MongoDB · Pipecat, Deepgram, Sarvam, ElevenLabs, Twilio · React, Next.js, React Native · Docker, AWS, Railway, Vercel

### Recognition

- 2nd place, internal Agentic AI Hackathon, Communication Crafts (2026)
- WOW Card as an intern, for shipping MarineDoc
- Bounty winner, [Aptos NFT Marketplace dApp](https://github.com/Amar5623/Aptos-NFT-Marketplace-Bounty)
