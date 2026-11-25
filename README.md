# Magic session planner API

NestJS API for managing Magic: The Gathering venues, scheduled sessions, nearby discovery, and seat allocation.

## Planned stack

NestJS and TypeScript, PostgreSQL with PostGIS, TypeORM migrations, and REST with OpenAPI. Authentication will support email magic links, Google, and Apple; the provider remains undecided. Seat requests require host approval. At session creation, the host chooses whether to play, which is the default, or only provide the table without occupying a seat. Session participation changes use database transactions to prevent overbooking.

## Development plan

Start with the [shared development plan](../magic-session-planner-docs/README.md), then follow the [development roadmap](../magic-session-planner-docs/development-roadmap.md). The documentation is maintained in the separate `magic-session-planner-docs` repository. Clone it alongside this repository to use these relative links locally.

This repository has been initialized on `main`. Framework setup, dependency installation, and application code are planned for roadmap step 1; there are no run or build commands yet.
