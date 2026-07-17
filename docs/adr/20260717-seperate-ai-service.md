# Separate the AI service

- Status: accepted
- Date: 2026-07-17

## Context and Problem Statement

The project includes AI-related functionality that has different runtime, dependency, and scaling needs from the web frontend and main API. We need to decide whether AI logic should live inside the main backend or in a separate service boundary.

## Considered Options

- Separate Python AI service
- Keep AI logic inside the main Node.js backend
- Use an external managed AI platform only

## Decision Outcome

Chosen option: "Separate Python AI service"
 - It isolates the AI stack from the main application, keeps dependency management cleaner, and allows the AI component to evolve independently.

## Links 

- [Tech stack](../techStack.md)
- [Monorepo ADR](20260717-use-monorepo.md)