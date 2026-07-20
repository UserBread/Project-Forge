# Use PostgreSQL for the database

- Status: accepted
- Date: 2026-07-17

## Context and Problem Statement

The project needs a durable relational database that supports structured application data, transactional integrity, and future growth. We also want a database with strong ecosystem support for Node.js applications and common deployment environments.

## Considered Options

- PostgreSQL
- MySQL
- SQLite

## Decision Outcome

Chosen option: "PostgreSQL"
 - It is familiar, offers strong relational features, reliable transactions, and broad tooling support while remaining a good fit for the planned backend stack.

## Links 

- [Tech stack](../techStack.md)
- [Monorepo ADR](20260717-use-monorepo.md)