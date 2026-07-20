# Use feature branches with pull requests for git workflow

- Status: proposed
- Date: 2026-07-20

## Context and Problem Statement

The repository will be worked on by multiple components and may involve changes across frontend, backend, AI, and infrastructure code. We need a Git workflow that keeps changes reviewable, works well with GitHub Actions, and avoids long-lived divergence between branches.

## Considered Options

- Feature branches with pull requests
- Trunk-based development
- GitFlow

## Decision Outcome

Chosen option: "Feature branches with pull requests"
 - It provides a simple review process, keeps history easy to follow, fits the expected pace of work for this monorepo, and works well with a protected main branch.

## Links 

- [Monorepo ADR](20260717-use-monorepo.md)
- [Tech stack](../techStack.md)
