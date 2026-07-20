# Technology Stack

## Frontend

| Technology     | Purpose        |
| -------------- | -------------- |
| React          | User Interface |
| TypeScript     | Type Safety    |
| Vite           | Build Tool     |
| Tailwind CSS   | Styling        |
| React Router   | Routing        |
| TanStack Query | Server State   |
| Zustand        | Client State   |
| Axios          | HTTP Client    |

---

## Backend

| Technology        | Purpose            |
| ----------------- | ------------------ |
| Node.js           | Runtime            |
| Express           | REST API           |
| TypeScript        | Type Safety        |
| Prisma            | ORM                |
| PostgreSQL        | Primary Database   |
| Redis *(planned)* | Caching & Sessions |

---

## AI Service

| Technology            | Purpose         |
| --------------------- | --------------- |
| Python                | AI Runtime      |
| FastAPI               | AI API          |
| Transformers          | LLM Integration |
| Sentence Transformers | Embeddings      |
| PyPDF / pdfplumber    | Resume Parsing  |

---

## Infrastructure

| Technology            | Purpose                 |
| --------------------- | ----------------------- |
| Docker                | Containerisation        |
| Docker Compose        | Local Development       |
| GitHub Actions        | CI/CD                   |
| Nginx *(planned)*     | Reverse Proxy           |
| Kubernetes *(future)* | Container Orchestration |

---

## Testing

| Technology            | Purpose             |
| --------------------- | ------------------- |
| Vitest                | Frontend Unit Tests |
| React Testing Library | Component Testing   |
| Jest                  | Backend Testing     |
| Supertest             | API Testing         |
| Playwright            | End-to-End Testing  |

---

## Documentation

* Markdown
* Architecture Decision Records (ADRs)
* Draw.io / Excalidraw diagrams
* GitHub Issues
* GitHub Projects
* GitHub Milestones

---

## Development Principles

* Type-safe development
* REST-first API design
* Modular architecture
* Separation of concerns
* Testable components
* Secure by default
* Containerised development
* Documentation-first workflow

---

## Planned Future Technologies

* Vector Database (Qdrant or pgvector)
* Retrieval-Augmented Generation (RAG)
* OpenTelemetry
* Prometheus
* Grafana
* Object Storage (S3 compatible)
* Terraform
* Cloud deployment (AWS or Azure)

---

## High-Level Architecture

```
React Frontend
        │
        ▼
Express REST API
   │          │
   ▼          ▼
PostgreSQL   AI Service (FastAPI)
                 │
                 ▼
      LLMs & Embedding Models
```
