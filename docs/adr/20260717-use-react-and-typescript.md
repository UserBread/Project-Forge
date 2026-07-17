# Use React and TypeScript for the frontend

- Status: proposed
- Date: 2026-06-23

## Context and Problem Statement

The project needs a frontend stack that supports a maintainable user interface, shared typing with backend services, and a good developer experience as the application grows. We also want a stack that works well with the monorepo structure and can support future expansion without major rewrites.

## Decision Drivers

- Strong type safety between UI code and shared models
- Good ecosystem support for component-based user interfaces
- Maintainability as the frontend grows
- Compatibility with the rest of the planned stack
- Familiarity and hiring availability

## Considered Options

- React with TypeScript
- React with JavaScript
- Vue with TypeScript
- Svelte with TypeScript

## Decision Outcome

Chosen option: "React with TypeScript"
 - It is familiar, provides a strong balance of ecosystem maturity, type safety, long-term maintainability, and alignment with the rest of the project’s tooling.

### Positive Consequences

- Shared types can be reused across frontend and backend
- TypeScript reduces runtime mistakes and improves refactoring safety
- React has a large ecosystem and broad community support
- Component-based architecture fits a modular frontend structure

### Negative Consequences

- TypeScript adds some initial setup and compile-time overhead
- React code can become overly abstract if patterns are not kept simple
- The team must maintain consistent typing discipline to get the full benefit

## Links

- [Tech stack](../techStack.md)
- [Monorepo ADR](20260717-use-monorepo.md)