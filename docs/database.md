# Database Design

## Overview

Project-Forge uses a relational database to store structured application data.

The database has been designed to prioritise:

* Data integrity
* Normalisation
* Scalability
* Query performance
* Maintainability

The primary database technology is PostgreSQL.

---

# Core Entities

The following entities form the foundation of the application.

## User

Stores:

* Account details
* Authentication information
* Preferences

Relationships:

* One Profile
* Many Resumes
* Many Applications
* Many Interviews

---

## Profile

Stores:

* Education
* Experience
* Skills
* Certifications
* Career Goals

---

## Resume

Stores:

* Uploaded document
* Version history
* Metadata
* AI analysis results

---

## Job

Stores:

* Company
* Title
* Description
* Salary
* Location
* Required Skills

---

## Application

Represents a user's application to a job.

Tracks:

* Status
* Dates
* Notes
* Interview progression

---

## Interview

Stores:

* Scheduled interviews
* Feedback
* AI evaluations
* Preparation history

---

## Skill

Stores individual technical and professional skills.

Examples:

* React
* Docker
* Kubernetes
* AWS
* Communication

Skills can belong to both users and jobs.

---

# High-Level Relationships

```text
User
 │
 ├── Profile
 │
 ├── Resume
 │
 ├── Application ─────── Job
 │                        │
 │                        │
 ├── Interview            │
 │                        │
 └────────────── Skills ──┘
```

---

# Future Entities

The database is expected to expand with additional entities.

Examples include:

* Learning Resources
* Career Roadmaps
* Notifications
* AI Conversations
* Saved Jobs
* Companies
* Recruiters
* Resume Versions
* Analytics Events

---

# Design Principles

The database follows these principles:

* Third Normal Form where appropriate
* Primary and foreign keys
* Indexed search fields
* UUID identifiers
* Soft deletes where necessary
* Audit timestamps
* Minimal data duplication

---

# Naming Conventions

Tables:

* Singular nouns

Columns:

* camelCase or snake_case (consistent throughout)

Primary Keys:

* id

Foreign Keys:

* entityId

Timestamps:

* createdAt
* updatedAt

---

# Migration Strategy

Schema changes will be managed through Prisma migrations.

Each migration should:

* Be reversible where practical
* Preserve existing data
* Be documented

---

# Future Improvements

Planned database enhancements include:

* Full-text search
* Vector embeddings
* Redis caching
* Read replicas
* Partitioning
* Analytics warehouse

---

# Entity Relationship Diagram

A detailed ERD will be maintained separately within the documentation folder.

This document provides the conceptual database design rather than the implementation details.
