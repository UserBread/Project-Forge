# Artificial Intelligence Design

## Overview

Project-Forge uses Artificial Intelligence to enhance the job-seeking process by analysing resumes, understanding job descriptions, identifying skill gaps, and providing personalised career guidance.

The AI components are designed as an independent microservice, allowing models and frameworks to evolve without affecting the core application.

---

## Goals

The AI system should:

* Parse uploaded resumes
* Extract structured information from unstructured documents
* Identify technical and soft skills
* Match candidates with suitable jobs
* Explain why a job is or is not a good fit
* Generate tailored resume improvements
* Generate cover letters
* Provide interview preparation
* Recommend learning paths

---

# AI Architecture

```
Frontend

↓

Node.js API

↓

AI Service (FastAPI)

↓

LLMs / Embedding Models

↓

Response

↓

Database
```

---

# Planned Features

## Resume Parsing

Extract:

* Personal Information
* Education
* Work Experience
* Skills
* Certifications
* Projects
* Languages

---

## Resume Intelligence

Analyse:

* ATS compatibility
* Missing skills
* Weak sections
* Actionable improvements

---

## Job Matching

Compare resumes against job descriptions using semantic similarity.

Output:

* Match Score
* Missing Skills
* Strengths
* Weaknesses
* Improvement Suggestions

---

## Career Coach

Provide personalised recommendations based on:

* Existing skills
* Desired career
* Previous applications
* Current market demand

---

## Interview Assistant

Generate:

* Technical questions
* Behavioural questions
* Follow-up questions

Evaluate:

* Communication
* Technical understanding
* STAR responses

---

## Future Enhancements

* Retrieval-Augmented Generation (RAG)
* Multi-Agent AI
* Voice Interviews
* Career Prediction Models
* Salary Prediction
* Learning Recommendation Engine

---

# Design Principles

* AI should explain its decisions whenever possible.
* AI should augment user decisions rather than replace them.
* AI components should remain independent from the core API.
* Models should be replaceable with minimal architectural changes.

---

# Current Status

Planning Phase

Future implementation details will be documented as Architectural Decision Records (ADRs).

---