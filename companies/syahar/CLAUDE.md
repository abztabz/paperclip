# Syahar — CEO Operating Workflow (remember this)

This file is the canonical, durable record of how Syahar is run. Treat every rule
here as standing unless the user (CEO) changes it. The committed package on branch
`claude/ceo-execution-plan-1p0q0i` is the **source of truth**; the live control
plane is an ephemeral demo.

## 🎯 Current scope: YEAR 1 (Phase 1 — Validate) ONLY
CEO directive (2026-06-16): focus on Year 1 only. Do **not** spin up Phase 2–5 work, 5-year automation build-outs, or later-phase hires unless asked. Year-1 objective: prove diaspora families pay for managed in-patient care and caregivers deliver to standard — **150 placements, ≥4.5★, ≥70% caregiver retention, contribution-positive, ≥1 organic-referral corridor — within the NPR 1.25cr budget.** 5-year strategy work (deck projections, opex automation plan) is parked as reference, not active.

## ⭐ Golden rules (non-negotiable)
1. **Positioning:** Syahar is a **cross-border caregiver platform** — peace of mind for diaspora families with hospitalised/ageing parents in Nepal. It is **NEVER** a remittance / money-transfer / FX service. Payment brands (IME, eSewa, Khalti, PSPs) are **partners and audience signals, never our product or competitors.** Every deliverable must sell care; correct any drift before use. (Enforced in COMPANY.md + all marketing agents.)
2. **Budget approval:** seek explicit CEO approval **before disbursing any budget** (model spend or cash). Roll back unapproved disbursements. Running agents on the OAuth **subscription** = $0 metered (it consumes subscription usage/limits, not money), but still get approval before running.

## Recurring cadence
3. **UK market intelligence** is the active focus (all other corridors paused). Produce a numbered report **every ~3 hours** (best-effort heartbeat) or **on demand** when the user says "refresh":
   - Verified secondary data only (ONS/Census, World Bank, Nepal care pricing) + transparent analyst model. **No live polling** — never fabricate survey numbers.
   - Write to `projects/uk-market-intelligence/documents/uk-market-report-NN.md`, note deltas vs prior report, commit + push, and send via `SendUserFile` (status proactive).
   - Reset `/tmp/uk-report-last.ts` and re-arm the heartbeat monitor after each report. Re-arm whenever it lapses; don't narrate every lapse.
4. **At every report instance → revise the marketing plan** (`projects/pre-launch-marketing/documents/pre-launch-brand-awareness-plan.md`) to match the findings, with a §0 changelog entry. Send the updated plan too.
5. **Show every marketing document the moment it's produced** — via the doc watcher (best-effort) and behaviorally (always, since the CEO triggers agent runs). Deliver with `SendUserFile`.

## Operating mechanics
6. **Branch & delivery:** develop on `claude/ceo-execution-plan-1p0q0i`; commit + push each deliverable (retry push up to 4× with backoff). Never open a PR unless asked.
7. **Collation:** all documents live under `companies/syahar/projects/<slug>/documents/` with a `PROJECT.md` index. Projects so far: `phase-1-validate`, `pre-launch-marketing`, `uk-market-intelligence`.
8. **Live control plane (ephemeral — rebuild on container resume):**
   - Postgres: native cluster, data dir `/tmp/seva-pgdata`, run as `postgres` OS user (initdb refuses root). Clear stale `postmaster.pid` if start fails.
   - Server: `cd server && IS_SANDBOX=1 DATABASE_URL=postgres://paperclip:paperclip@127.0.0.1:5432/paperclip PORT=3100 HOST=127.0.0.1 BETTER_AUTH_SECRET=… node --import tsx src/index.ts` — launch via the harness background mechanism (it keeps the process alive). `IS_SANDBOX=1` is **required** so the claude_local adapter can run `claude --dangerously-skip-permissions` as root.
   - Company `Syahar` id `e170de2a-666b-4bfb-8b2f-41e54d2b23f6`. Agents: ceo `d9caaed7`, marketing-lead `9ffe9045`, content-community `dcca1503`, creative-copy `cf054e71`, growth-outreach `d31976c0`, + legal/recruiter/coordinator/engineer.
   - Run an agent: `IS_SANDBOX=1 pnpm paperclipai heartbeat run -a <agentId> --api-base http://127.0.0.1:3100`.
9. **Honesty:** report real status (infra down, subscription session-limit hits, "documents are drafts not executed actions" — no real FB page/ads/proposals-sent until a human acts). Don't overclaim.

## Org
CEO → {Legal & Compliance, Recruiter/QA, Lead Engineer, Care Coordinator, Marketing Lead}; Marketing Lead → {Content & Community, Creative & Copy, Growth & Outreach}. Agents are equipped with vendored marketing skills (MIT, in `skills/`).

## Open items (carry forward)
- Pre-launch marketing spend approval (NPR 250k tranched) — awaiting CEO.
- `abztabz/syahar-app` (the product app) — out of session scope; needs adding to work on it (SYA-2).
- True unattended scheduling needs a persistent deployment (cron/wakeup tools not available in-session).
