# Hi, I'm Vinayak Tiwari 👋

### Backend & AI Systems Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/vinayak-tiwari-2357a9371)
[![Portfolio](https://img.shields.io/badge/Portfolio-06B6D4?style=flat&logo=react&logoColor=white)](https://portfolio-eosin-six-cg0cj01myh.vercel.app/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:tiwarivinayak859@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/VinayakTiwari7)

I build **AI-powered applications, backend systems, and developer infrastructure** with a focus on practical engineering, clean APIs, and production-oriented design.

Currently pursuing a **B.Tech in Computer Engineering** at Shah & Anchor Kutchhi Engineering College, with hands-on experience building systems around **LLMs, RAG, agentic workflows, asynchronous APIs, and enterprise backend services.**

---

##  What I Build

| Area | Focus |
| :--- | :--- |
|  **AI Systems & Agents** | LLM applications, RAG, LangGraph state machines, tool calling, vector search |
|  **AI Infrastructure** | Provider abstraction gateways, SSE streaming, circuit breakers, failover pipelines |
|  **Backend & Microservices** | FastAPI, Spring Boot 3, Spring Security, JWT RBAC, async architectures |
|  **Full Stack Systems** | React 18/19, TypeScript, Tailwind CSS, API-driven single-page applications |

---

##  Featured Projects

### 1. [Cortex — AI Orchestration Gateway](https://github.com/VinayakTiwari7/cortex)

[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)](https://redis.io)
[![Pydantic](https://img.shields.io/badge/Pydantic-v2-E92063?style=flat&logo=pydantic&logoColor=white)](https://docs.pydantic.dev/)
[![Render](https://img.shields.io/badge/Render-Deployed-46E3B7?style=flat&logo=render&logoColor=black)](https://cortex-rnhl.onrender.com/)

A resilient, provider-agnostic async API gateway built with FastAPI that unifies multiple LLM providers (Groq, Gemini) behind a single normalized interface with automatic failover, circuit breaking, and caching.

- **Abstract Provider Interface**: Normalized `complete()` and `stream()` contracts via Python `ABC`.
- **Pre-Stream Commit Failover**: Transparently retries against fallback providers before committing HTTP response headers.
- **First-Principles Circuit Breaker**: Closed/Open/Half-Open state machine to isolate failing providers and test recovery.
- **Redis Response Caching & Rate Limiting**: Atomic `INCR`/`EXPIRE` operations designed to fail-open gracefully.

🔗 **[Live Application](https://cortex-rnhl.onrender.com/)** • **[Interactive API Docs](https://cortex-rnhl.onrender.com/docs)** • **[GitHub Repository →](https://github.com/VinayakTiwari7/cortex)**

---

### 2. [Nexus — Autonomous Agentic RAG Assistant](https://github.com/VinayakTiwari7/nexus)

[![LangGraph](https://img.shields.io/badge/LangGraph-StateGraph-FF6F00?style=flat&logo=langchain&logoColor=white)](https://langchain-ai.github.io/langgraph/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=flat&logo=google&logoColor=white)](https://ai.google.dev/)
[![ChromaDB](https://img.shields.io/badge/Vector_DB-ChromaDB-FFA000?style=flat)](https://trychroma.com)
[![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?style=flat&logo=docker&logoColor=white)](https://docker.com)
[![Tests](https://img.shields.io/badge/Pytest-44%20Passed-brightgreen?style=flat&logo=pytest&logoColor=white)](https://docs.pytest.org)

An autonomous AI assistant coupling persistent vector embeddings with a LangGraph StateGraph agent for multi-step tool execution, grounded RAG retrieval, and order tracking.

- **Cyclical StateGraph Workflow**: Dynamic routing across document search, order lookup, and safe AST calculator tools.
- **Grounded Vector Search**: Persistent ChromaDB store using Gemini `text-embedding-004` and hierarchical chunking.
- **Prompt-Injection Defense**: Strict system prompt grounding with application-controlled verifiable citations.
- **Dual Runtime Architecture**: Live Gemini function calling with deterministic offline fallbacks for automated testing.

🔗 **[Live Application](https://nexus-upp2.onrender.com)** • **[GitHub Repository →](https://github.com/VinayakTiwari7/nexus)**

---

### 3. [SmartHire — Full-Stack Employee Onboarding Platform](https://github.com/VinayakTiwari7/smarthire)

[![Java 17](https://img.shields.io/badge/Java-17-ED8B00?style=flat&logo=openjdk&logoColor=white)](https://openjdk.org)
[![Spring Boot 3](https://img.shields.io/badge/Spring_Boot-3.3-6DB33F?style=flat&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Spring Security](https://img.shields.io/badge/Spring_Security-6.x-6DB33F?style=flat&logo=springsecurity&logoColor=white)](https://spring.io/projects/spring-security)
[![JWT](https://img.shields.io/badge/Auth-JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)](https://jwt.io)
[![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat&logo=mysql&logoColor=white)](https://mysql.com)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=flat&logo=react&logoColor=black)](https://react.dev)

A layered Spring Boot 3 REST API and React SPA for employee onboarding, task assignments, and overdue tracking with role-based access control.

- **Layered Architecture**: Strict `Controller → Service → Repository` separation with DTO-only responses and global exception envelope.
- **Three-Tier RBAC**: Granular endpoint authorization (`Admin`, `Manager`, `Employee`) enforced via `@PreAuthorize`.
- **Automated Overdue Detection**: Custom JPQL queries auto-surfacing pending and overdue employee onboarding tasks.
- **Production Cloud Deployment**: Backend deployed to Railway with MySQL plugin; frontend hosted on Vercel.

🔗 **[Live Frontend](https://smarthire-frontend-sooty.vercel.app)** • **[Swagger UI API](https://smarthire-production-9543.up.railway.app/swagger-ui.html)** • **[GitHub Repository →](https://github.com/VinayakTiwari7/smarthire)**

---

### 4. [Campus Lost & Found Portal](https://github.com/VinayakTiwari7/Lost_found_Portal)

[![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248?style=flat&logo=mongodb&logoColor=white)](https://mongodb.com)
[![Express.js](https://img.shields.io/badge/Express.js-Backend-000000?style=flat&logo=express&logoColor=white)](https://expressjs.com)
[![React](https://img.shields.io/badge/React-Frontend-61DAFB?style=flat&logo=react&logoColor=black)](https://react.dev)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-3.4-38B2AC?style=flat&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)

A full-stack MERN platform featuring a 15+ endpoint REST API, claim-based recovery workflows, Multer image uploads, and admin moderation analytics.

🔗 **[Live Demo](https://lost-found-portal-two.vercel.app)** • **[GitHub Repository →](https://github.com/VinayakTiwari7/Lost_found_Portal)**

---

##  Technical Stack

### **Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=c%2B%2B&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat&logo=postgresql&logoColor=white)

### **AI & Agentic Systems**
![LangGraph](https://img.shields.io/badge/LangGraph-FF6F00?style=flat&logo=langchain&logoColor=white)
![Gemini API](https://img.shields.io/badge/Google_Gemini-4285F4?style=flat&logo=google&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FFA000?style=flat)
![RAG](https://img.shields.io/badge/RAG_Pipelines-0055FF?style=flat)
![SSE](https://img.shields.io/badge/SSE_Streaming-06B6D4?style=flat)

### **Backend & APIs**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat&logo=springsecurity&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat&logo=express&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic_v2-E92063?style=flat&logo=pydantic&logoColor=white)
![AsyncIO](https://img.shields.io/badge/AsyncIO-3776AB?style=flat&logo=python&logoColor=white)

### **Databases & Caching**
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)

### **Frontend**
![React](https://img.shields.io/badge/React_18/19-61DAFB?style=flat&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwindcss&logoColor=white)

### **Tools & Cloud Platforms**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat&logo=pytest&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=black)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat&logo=railway&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)

---

##  Engineering Focus

I specialize in systems engineering at the intersection of:

$$\text{Backend Engineering} \times \text{AI Systems}$$

- **Agentic Workflows**: Multi-turn cyclical StateGraphs, tool evaluation, and AST reasoning.
- **Fail-Safe Gateways**: Circuit breaking, graceful cache degradation, and multi-provider failover routing.
- **Deterministic RAG**: Citation grounding, prompt-injection defense, and verifiable regression suites.
- **Layered Architecture**: Spring Boot microservices, RBAC security, and clean DTO contracts.

---

##  Connect With Me

- **LinkedIn**: [linkedin.com/in/vinayak-tiwari-2357a9371](https://linkedin.com/in/vinayak-tiwari-2357a9371)
- **Portfolio**: [portfolio-eosin-six-cg0cj01myh.vercel.app](https://portfolio-eosin-six-cg0cj01myh.vercel.app/)
- **Email**: [tiwarivinayak859@gmail.com](mailto:tiwarivinayak859@gmail.com)
- **Location**: Mumbai, India
