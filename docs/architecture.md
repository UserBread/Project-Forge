# Project-Forge Architecture

## Overview

Project-Forge follows a modular service-oriented architecture designed to separate responsibilities between the user interface, application logic, artificial intelligence, and data persistence.

The goal of this architecture is to maximise maintainability, scalability, testability, and future extensibility.

---

# High-Level Architecture

```text
                    ┌──────────────────────┐
                    │   React Frontend     │
                    └──────────┬───────────┘
                               │
                         HTTPS / REST
                               │
                    ┌──────────▼───────────┐
                    │  Express REST API    │
                    └──────┬─────────┬─────┘
                           │         │
                 Database  │         │ AI Requests
                           │         │
              ┌────────────▼───┐   ┌─▼────────────────┐
              │ PostgreSQL      │   │ FastAPI AI       │
              │                 │   │ Service          │
              └─────────────────┘   └──────┬──────────┘
                                            │
                               Embeddings / LLMs / NLP
```

---

# Design Principles

The architecture is built around the following principles:

* Separation of concerns
* Modular components
* Independent AI services
* Loose coupling
* High cohesion
* Type safety
* Documentation-first development
* Security by default

---

# Application Layers

## Presentation Layer

Responsibilities:

* User Interface
* Forms
* Authentication
* Dashboard
* Resume Management
* Job Tracking

Technology:

* React
* TypeScript

---

## API Layer

Responsibilities:

* Authentication
* Validation
* Business Logic
* Database Communication
* AI Service Communication

Technology:

* Express
* TypeScript

---

## AI Layer

Responsibilities:

* Resume Parsing
* Resume Analysis
* Job Matching
* Career Coaching
* Interview Preparation

Technology:

* FastAPI
* Python

---

## Data Layer

Responsibilities:

* Persistent storage
* Query optimisation
* Relationships
* Data integrity

Technology:

* PostgreSQL
* Prisma

---

# Planned Modules

* Authentication
* User Profiles
* Resume Management
* Job Management
* Application Tracking
* AI Services
* Analytics
* Administration

---

# Communication

Frontend communicates only with the REST API.

The REST API is responsible for:

* Validation
* Authentication
* Business Logic

The AI Service communicates only with the API and is never exposed directly to clients.

---

# Future Architecture

Future versions may include:

* Redis caching
* Background workers
* Vector database
* Object storage
* Kubernetes deployment
* Event-driven processing
* Message queues

---

# Non-Functional Goals

* Responsive user interface
* Secure authentication
* Horizontal scalability
* High maintainability
* High test coverage
* Containerised deployment
* Clear documentation

---

# Architecture Evolution

This document represents the intended architecture.

Architectural changes will be recorded through Architecture Decision Records (ADRs).
