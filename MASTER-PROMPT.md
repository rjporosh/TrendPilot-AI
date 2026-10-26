# Master Implementation Prompt — TrendPilot AI

Act as a senior software architect and implementation engineer. Build TrendPilot AI as a complete, tested, documented Python application for original Bengali short-form video production and publishing across YouTube, Facebook and Instagram.

Do not return only pseudocode or a plan. Inspect the repository, implement the application, run tests, fix failures, and document the actual results.

### Required Stack

Python, FastAPI, SQLite, SQLAlchemy, Pydantic Settings, httpx, FFmpeg, pytest, and optional n8n.

### Required Modules

* Trend research and multi-niche scoring
* AI provider abstraction and scriptwriter
* Storyboard and visual generation adapters
* Bengali TTS and subtitle generation
* FFmpeg video rendering
* Asset-rights ledger and content-quality gates
* YouTube publishing adapter
* Facebook and Instagram publishing adapters
* OAuth connection and permission diagnostics
* Scheduling, retries and duplicate prevention
* Analytics and cost tracking
* Responsive dashboard
* Logs, audit trail and global emergency stop

### Non-Negotiable Requirements

1. Do not guess which AI service provides the user's one-billion-token allowance. Implement a provider interface and mock adapter until the exact provider is confirmed.
2. Never request social account passwords.
3. Use documented official APIs and OAuth only.
4. Treat social URLs as destinations, not authorization.
5. Keep public auto-publishing disabled until the owner has completed integration and safety tests.
6. Missing asset-license evidence or a critical quality failure must block publishing.
7. Never create fake engagement, bypass platform rules, or republish other creators' videos with minor changes.
8. Add hard daily budget and upload limits, retries, idempotency and a global stop switch.
9. Never promise monetization or guaranteed income.
10. Keep credentials, tokens, private generated media and local databases out of Git.

### Development Sequence

1. Create the project foundation and database.
2. Implement mock providers and health checks.
3. Build an end-to-end script-to-video workflow.
4. Implement rendering and quality checks.
5. Add a dry-run publishing system.
6. Add official YouTube integration.
7. Add official Facebook and Instagram integrations.
8. Add analytics, scheduler and bounded automation.
9. Create a responsive dashboard.
10. Run tests and update README, release notes and AI handover.

### Definition of Done

The app must run on macOS from documented commands, render a sample vertical MP4, support demo mode, block unsafe publishing, prevent duplicate uploads, enforce budgets, and pass its tests.

Clearly distinguish implemented functionality, mocked functionality, unverified integrations and manual account-approval requirements.

At completion, report files created, installation commands, tests and results, required account setup, known limitations and next steps.
