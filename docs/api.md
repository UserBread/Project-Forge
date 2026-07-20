# API Overview

## Purpose

The Project-Forge API provides a secure REST interface between the frontend, database, and AI services.

The API is responsible for:

* Authentication
* User management
* Resume management
* Job management
* Application tracking
* AI integration

---

# Architecture

```
React Frontend

↓

REST API

↓

Services

↓

Database
```

The AI Service communicates with the API through internal endpoints.

---

# Planned API Modules

## Authentication

Responsible for:

* Registration
* Login
* Logout
* Password Reset
* JWT Refresh

---

## Users

Responsible for:

* User profiles
* Experience
* Education
* Skills

---

## Resumes

Responsible for:

* Uploading
* Versioning
* Viewing
* Deleting
* AI Analysis

---

## Jobs

Responsible for:

* Searching
* Filtering
* Matching
* Recommendations

---

## Applications

Responsible for:

* Tracking application progress
* Notes
* Interview scheduling
* Status updates

---

## AI

Responsible for:

* Resume parsing
* Resume scoring
* Job matching
* Career coaching
* Interview generation

---

# API Standards

* RESTful endpoints
* JSON request/response bodies
* JWT Authentication
* Versioned routes (`/api/v1`)
* Consistent error responses
* Input validation
* Rate limiting

---

# Security

The API will implement:

* JWT authentication
* Role-based authorisation
* Request validation
* File validation
* HTTPS in production
* Rate limiting

---

# Testing

The API will be tested using:

* Unit Tests
* Integration Tests
* End-to-End Tests

---

# Current Status

Planning Phase.
