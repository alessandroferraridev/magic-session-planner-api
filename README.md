# Magic session planner API

NestJS API for managing Magic: The Gathering venues, scheduled sessions, nearby discovery, and seat allocation.

## Planned stack

NestJS and TypeScript, PostgreSQL with PostGIS, TypeORM migrations, and REST with OpenAPI. Authentication uses Google and Apple only, integrated directly with NestJS-owned users and sessions; explicit linking and immediate revocation follow the shared authentication specification. The audience is 18+ by self-declaration. Deploy to Vercel Hobby with Neon Free PostgreSQL/PostGIS; use Workflow/Nest and Expo push for durable notifications without polling. Discovery is city-only and exact location is restricted to hosts/approved participants. Seat requests require host approval. At session creation, the host chooses whether to play, which is the default, or only provide the table without occupying a seat. Session participation changes use database transactions to prevent overbooking.

## Development plan

Start with the [shared development plan](../magic-session-planner-docs/README.md), then follow the [development roadmap](../magic-session-planner-docs/development-roadmap.md). The documentation is maintained in the separate `magic-session-planner-docs` repository. Clone it alongside this repository to use these relative links locally.

Use feature branches from the protected default `dev` branch and pull requests; `main` contains release milestones. Framework setup, dependency installation, and application code are planned for roadmap step 1; there are no run or build commands yet.

See the [accepted authentication policy](../magic-session-planner-docs/authentication.md), [operating/retention policy](../magic-session-planner-docs/operations.md), and [implementation roadmap](../magic-session-planner-docs/development-roadmap.md). Only the initial format catalogue remains open. Unit, integration and E2E suites are required from scaffolding; none exists yet.
