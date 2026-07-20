# Use Prisma for the ORM

- Status: proposed
- Date: 2026-07-20

## Context and Problem Statement

The backend needs a database access layer that works well with TypeScript, supports migrations, and keeps application code maintainable as the schema evolves. We want a solution that fits the planned PostgreSQL database and reduces low-level SQL boilerplate where possible.

## Considered Options

- Prisma
- Raw SQL with a query builder
- Another ORM such as TypeORM or Sequelize

## Decision Outcome

Chosen option: "Prisma"
 - It provides strong TypeScript support, a clear migration workflow, and a good fit for PostgreSQL in this codebase.

## Links 

- [PostgreSQL ADR](20260717-use-postgressql.md)
- [Tech stack](../techStack.md)
