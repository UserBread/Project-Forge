# Use Docker for local development

- Status: proposed
- Date: 2026-07-20

## Context and Problem Statement

The project includes multiple services and supporting infrastructure that need to work together during development. We need a local setup that is repeatable, easy to start, and close to the eventual deployment shape.

## Considered Options

- Docker Compose for local development
- Run each service directly on the host machine
- Use a custom development script or task runner only

## Decision Outcome

Chosen option: "Docker Compose for local development"
 - It makes it easier to start the required services consistently and reduces environment-specific setup issues.

## Links 

- [Monorepo ADR](20260717-use-monorepo.md)
- [Tech stack](../techStack.md)
