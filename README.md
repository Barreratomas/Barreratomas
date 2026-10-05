# Hi, I'm Tomás 👋

Software Engineer focused on backend systems and production-grade LLM agents.
I build the backend that keeps things running (queues, real-time processing, CI/CD, deploys that
roll back on their own) and the AI systems that live on top of it. I like taking things from
prototype to production with full ownership.

When I'm not building, I'm probably redesigning something that shouldn't exist the way it does,
or eliminating a deadlock nobody knew was there.

---

## Backend & systems

- Design and rebuild backends in layered and hexagonal architectures (Node.js/Express, FastAPI, Laravel),
  including a legacy production system where I eliminated the deadlocks that froze it
- Move heavy work to async job queues with parallel ETLs and real-time progress over WebSockets/Socket.IO
  (a ~30 min process down to ~13 min)
- Build reliable messaging infrastructure for the WhatsApp Business API: durable Redis queues with
  acknowledgment, persistent debouncing and idempotency, so a deploy doesn't lose messages
- Build multi-tenant platforms and real-time engines, like a location and availability-based
  assignment engine with 500+ bookings, still in production
- Take systems from zero to automated delivery: Git, Docker, GitHub Actions CI/CD, health checks,
  automatic rollback and secrets management
- Secure APIs with JWT, bcrypt and parameterized SQL; integrate payments (Mercado Pago subscriptions) and Google Maps

## AI & agents

- Design multi-agent systems with LangGraph: conditional routing, HITL, episodic memory
- Build production WhatsApp agents as a 4-layer pipeline (interpreter, decider, writer, critic): the LLM
  decides the action, while prices and medical info are inserted verbatim from the knowledge base
- Put guardrails around the model that don't depend on it: health gates, response filters, and a critic
  that can veto risky answers
- Build RAG pipelines with Qdrant and ChromaDB, evaluated against golden sets
- Implement Text-to-SQL, schema linking and anti-prompt-injection defense in production
- Fine-tune models with LoRA (mDeBERTa, multilingual classification)

---

## Selected work

- [WhatsApp sales agent for an aesthetics business](https://github.com/Barreratomas/whatsapp-sales-agent-case-study) (client project, private repo): durable queue,
  4-layer LangGraph pipeline, 21 services, 1000+ tests, automated deploys with rollback
- [Karlook](https://www.karlook.io/): real-time assignment engine for mobile car washes, Mercado Pago subscriptions
- [EMACE](https://github.com/Barreratomas/EMACE): multi-tenant, hub-and-spoke multi-agent platform
  on LangGraph with hexagonal architecture
- [Fake News Detection](https://github.com/Barreratomas/fakenews): mDeBERTa v3 + LoRA classifier
  combined with RAG fact-checking

---

## Main Stack

**Backend:** Python (FastAPI, Django), Node.js (Express, NestJS), Java (Spring Boot), PHP (Laravel)

**Databases & queues:** PostgreSQL, MySQL, SQL Server, MongoDB, Redis

**Architecture:** Hexagonal, Clean Architecture, Multi-Tenant, Event-Driven, MVC, REST, WebSockets

**Infra / DevOps:** Docker, GitHub Actions, AWS, Render, Linux, Nginx

**Testing:** Pytest, Jest

**AI / LLM:** LangGraph, LangChain, LangSmith, RAG, HITL, Text-to-SQL, Prompt Engineering

**ML / DL:** PyTorch, Transformers, LoRA, Scikit-learn, Pandas, NumPy

**Vector Stores:** Qdrant, ChromaDB, FAISS

**LLM Providers:** OpenAI, Gemini, Groq, OpenRouter, DeepSeek

---

## Contact

- 📧 tomesbarrera@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/tomastb/)
- 🌐 [Portfolio](https://landing-barreratomas-projects.vercel.app/)
