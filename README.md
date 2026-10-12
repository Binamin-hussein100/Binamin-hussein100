# Hi, I'm Binamin 👋

**Backend engineer moving into AI engineering.** I build APIs and microservices, ship them with Docker, Kubernetes and CI/CD, and now build retrieval and LLM systems in Python.

- 🔭 **Building:** an AI assistant for Kenyan health-cover documents that grows from RAG to an API service to an evaluated agent. I'm building it in public over 12 weeks.
- 🌱 **Learning:** AI engineering at Moringa School: evaluation, fine-tuning, LLMOps, agents and MCP
- 🤝 **Open to:** backend, DevOps and AI engineering roles and collaborations
- 💬 **Ask me about:** RAG pipelines, Node.js microservices, blue-green deployments on Kubernetes

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/binamin-hassan-0a7470208/)
[![X](https://img.shields.io/badge/@codivorous-000000?style=flat&logo=x&logoColor=white)](https://twitter.com/codivorous)

---

## 🧠 AI engineering

### [Custom-RAG](https://github.com/Binamin-hussein100/Custom-RAG): RAG from scratch, no framework
`Python` `SentenceTransformers` `FAISS` `Gemini`

- Full pipeline written by hand: PDF loading, overlapping chunks, embeddings, FAISS search, grounded generation
- Answers cite their sources (`[Source N: file | page]`) and say "I don't know" when the documents don't cover the question
- A SHA-256 manifest skips re-indexing unless the documents, embedding model or chunk settings change
- CLI with `ingest`, `ask` and `chat` commands, and a smoke test for every module

### [Multi_modal_RAG](https://github.com/Binamin-hussein100/Multi_modal_RAG): Q&A over PDFs with tables and images
`Python` `unstructured` `LangChain` `Chroma` `OpenAI`

- High-resolution layout parsing pulls text, tables (as HTML) and images out of PDFs
- A vision model turns tables and images into searchable descriptions, so they can be retrieved like plain text
- Deterministic chunk IDs make re-ingestion an update instead of a duplicate

### [RAG_Langchain](https://github.com/Binamin-hussein100/RAG_Langchain): conversational RAG with memory
`Python` `LangChain` `Chroma` `OpenAI`

- Rewrites follow-up questions into standalone search queries using the chat history, so "what about the second one?" still retrieves the right passages

---

## ⚙️ Backend & DevOps

### [E-commerce-API](https://github.com/Binamin-hussein100/E-commerce-API): Node.js microservices on Kubernetes
`Node.js` `Express` `Prisma` `PostgreSQL` `Docker` `Kubernetes` `GitHub Actions` `Jest`

- Six services (users, products, cart, orders, payments, notifications), each with its own PostgreSQL database through Prisma
- Blue-green deployments on Kubernetes with liveness and readiness probes, resource limits and multiple replicas, behind an NGINX ingress that routes by path
- GitHub Actions matrix pipeline builds and pushes a Docker image per service, tagged with the commit SHA, with Slack notifications on start, success and failure
- JWT authentication with role-based middleware, unit-tested with Jest

---

## 🛠️ Tech stack

**AI & data**<br>
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logo=meta&logoColor=white)
![Chroma](https://img.shields.io/badge/Chroma-FF6446?style=for-the-badge&logoColor=white)

**Backend**<br>
![Node.js](https://img.shields.io/badge/Node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-404D59?style=for-the-badge&logo=express&logoColor=61DAFB)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)

**DevOps**<br>
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

<sub>Also worked with: JavaScript, TypeScript, React, Angular, Ruby on Rails, MySQL, SQLite, Postman.</sub>

---

## 📈 Now shipping

| Week | Milestone | Status |
|---|---|---|
| 1 | Clean up repos, collect the Kenyan health-cover corpus | 🟡 In progress |
| 2–3 | RAG v1 with a 50-question evaluation set, recall@k and faithfulness scores | ⏳ Next |
| 4 | LoRA fine-tuned question router (English, Swahili, Sheng) and a live demo | ⏳ |
| 6–9 | FastAPI + MCP service, LangGraph agent, CI eval gates, security hardening | ⏳ |

---

![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Binamin-hussein100&layout=compact&hide_border=true&theme=nord)
