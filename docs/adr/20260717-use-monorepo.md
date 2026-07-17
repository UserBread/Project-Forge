# Use a monorepo for the repository structure

- Status: proposed
- Date: 2026-07-17

## Context and Problem Statement

This project contains multiple closely related parts: a web app, an API service, an AI service, shared packages, and infrastructure code. We need a repository structure that makes it easy to develop these pieces together, share code safely, and keep deployment boundaries clear.

## Decision Drivers

- Shared code between services should be easy to manage
- Local development should support running multiple components together
- Changes that span frontend, backend, and infrastructure should be coordinated in one place
- The repository should stay understandable as the project grows
- We want to avoid duplicated configuration and tooling across separate repos

## Considered Options

- Monorepo with separate apps and packages
- Multiple repositories, one per service
- Hybrid approach with shared libraries in a separate repository

## Decision Outcome

Chosen option: "Monorepo with separate apps and packages"
 - It best fits the current size and shape of the project. 
 - It keeps the web app, API, AI service, shared types, and infrastructure close together while still allowing clear boundaries between them.

### Positive Consequences

- Shared types and utilities can be reused without publishing packages early
- Cross-cutting changes are easier to make and review
- One set of repo-level tooling and conventions can be used
- Local setup and onboarding are simpler

### Negative Consequences

- The repository will be larger and more complex to navigate
- Tooling may need workspace-aware configuration
- Changes in one area can affect unrelated parts if boundaries are not enforced carefully

## Links

- [ADR template](ADR-template.md)