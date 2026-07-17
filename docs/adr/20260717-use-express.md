# Use ExpressJS for the backend

- Status: accepted
- Date: 2026-07-17

## Context and Problem Statement

The backend needs a lightweight HTTP framework that is easy to set up, fits well with a TypeScript codebase, and supports a modular API layer as the project grows. We want something simple enough for the current scope without locking us into unnecessary framework complexity.

## Considered Options

- ExpressJS
- Fastify
- NestJS

## Decision Outcome

Chosen option: "ExpressJS"
 - It is familiar, widely supported, and provides a minimal foundation for building the API without imposing a heavy framework structure.

## Links 

- [Tech stack](../techStack.md)
- [Monorepo ADR](20260717-use-monorepo.md)