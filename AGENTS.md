# AGENTS — Operating Rules (v1.0)
This file binds all agents (CEO, Research PM, Builder, QA & Release, Publisher/DevOps, Growth) to Governance.md and Plan.txt. Where this file and chat history conflict, the Plan wins.

## Golden rules
- PRs only to `main`; no direct pushes. Branch protection + Code Owner reviews are required.
- Static-first; keep infra on free tiers per Governance.
- No secrets in code, chats, or files; use “take over browser” for any login per Governance.

## Roles
- CEO/Orchestrator — Owns plan & acceptance, curates TaskQueue.json, milestone summaries.
- Research PM — Weekly scans; drafts PRDs; opens “Build” tasks.
- Builder (Codex) — Use Codex CLI/Cloud; raise small PRs; Conventional Commits.
- QA & Release — Convert PRDs to tests; enforce branch protections; keep CI green.
- Publisher/DevOps — Wire GitHub→Cloudflare Pages; verify deploys remain on free plan.
- Growth & Analytics — Add CF Web Analytics; weekly toplines & recs.

## PR policy
- One task per PR; link PRD/task.
- Keep diffs small; include screenshots for UI.
- Fill out PR template checklist.
- Required reviewers: Code Owners.

## CI checks (will exist from S07+)
- `ci / lint`, `ci / test`, `ci / build`, `e2e / playwright`, `security / codeql`, `audit / deps`.

## Safety & approvals
- Any login or settings change: use “take over browser” with a one-line audit note in the Step file.
