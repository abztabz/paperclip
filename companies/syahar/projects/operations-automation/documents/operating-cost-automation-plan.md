# Syahar — Operating Cost Automation Plan

**Owner:** CEO · **Prepared:** 2026-06-16 · **FX:** USD 1 ≈ NPR 133
**Thesis:** automate the knowledge-work layer with Claude agents (as proven with the marketing pod); keep a lean human core for physical care, ground relationships, and family trust.

---

## 1. Why operating cost is high

Year-5 opex is NPR 24.5cr. Two lines dominate:

| Cost line (Y5, NPR cr) | Amount | % of opex | Nature |
|---|---:|---:|---|
| **People / payroll** | 9.20 | **38%** | Coordinators, marketing, engineering, customer success, finance, ops mgmt — scales with cities/placements |
| **Marketing & acquisition** | 5.60 | **23%** | Acquisition labor + paid media |
| Caregiver supply, training & QA | 3.00 | 12% | Mostly physical (vetting, training) |
| Technology & product | 2.40 | 10% | Hosting, PSP, security — compute, not labor |
| Payments & FX infrastructure | 2.30 | 9% | A % of settlement volume — unavoidable |
| G&A, legal & compliance | 2.00 | 8% | Drafting, reporting, audit, admin |
| **Total** | **24.5** | 100% | |

The point: **People + Marketing = 61% of opex**, and most of it is *knowledge work that doesn't have to be human.* (The actual caregiving is pass-through, not opex — so cost reduction targets coordination/marketing/analytics/admin, not care.)

## 2. Automate / hybrid / keep-human map

| Function | Today (human) | Verdict | Claude agent / how | Keep human for |
|---|---|---|---|---|
| **Marketing** (content, creative, PR, referrals, analytics) | Marketing Mgr + team | **Automate** ✅ (done) | Content & Community, Creative & Copy, Growth & Outreach pod | media spend approval, key partnerships |
| **Customer success / retention** | CS hires | **Automate** | CS agent: NPS analysis, proactive flags, retention comms drafting | escalations, emotional moments |
| **Analytics / data** | Data Engineer | **Automate** | Analytics agent: dashboards, cohort/CAC/funnel, reporting | — |
| **Finance** | CFO + team | **Hybrid** | Finance agent: investor-grade models, board reporting, forecasting | fundraising relationships, signoff, audit |
| **Engineering** | Engineers ×N | **Hybrid** (force-multiplier) | Claude writes/maintains most code → fewer engineers per output | architecture, security ownership |
| **Ops coordination** (matching, scheduling, report compilation, escalation triage) | Care/City Coordinators | **Hybrid** | Coordinator agent automates the digital workflow | family reassurance, ground judgment |
| **Legal / compliance** | Counsel | **Hybrid** | Legal-research agent: drafting, compliance research, doc prep | signatures, regulator/court, liability |
| **Caregiver supply & QA** | Recruiter/QA | **Keep human** | scheduling/docs only | in-person vetting, health screening, training |
| **Caregivers** | Caregivers | **Keep human** | — | the care itself (pass-through cost) |
| **City presence / hospital MoUs** | City Coordinators | **Keep human** | — | on-the-ground relationships |
| **CEO / strategy / fundraising** | Founder | **Keep human** | — | judgment, investors, board |

**Principle:** automate the *back office and the keyboard*; keep humans on *the body, the relationship, and the trust.*

## 3. Re-modelled operating cost (Year 5, directional)

| Cost line (Y5, NPR cr) | Current | Automatable share | Lean target | Saving |
|---|---:|---:|---:|---:|
| People / payroll | 9.20 | ~45% (back-office) | ~5.1 | **~4.1** |
| Marketing & acquisition | 5.60 | ~40% (labor) | ~3.4 | **~2.2** |
| G&A, legal & compliance | 2.00 | ~25% (drafting/reporting) | ~1.5 | **~0.5** |
| Caregiver supply, training & QA | 3.00 | ~7% (coord/docs) | ~2.8 | ~0.2 |
| Technology & product | 2.40 | low (infra) | ~2.4 | ~0 |
| Payments & FX | 2.30 | none (volume %) | ~2.3 | 0 |
| **Total opex** | **24.5** | | **~17.5** | **~7.0** |

**Impact at Year 5:**
- Opex **24.5cr → ~17.5cr** (−~29%)
- Operating profit **16.9cr → ~23.9cr**
- Operating margin **41% → ~58%**
- Plus the same logic compresses Phases 2–4, pulling **full-year profitability earlier** (potentially into Phase 3) and **shrinking the external funding need** below the planned USD 2.6–3.0M.

*(Directional estimates; validate per phase against actuals. Automatable shares are deliberately conservative.)*

## 4. Guardrails (what automation must NOT do)
- **Don't automate the trust touch.** Phase 1 is manual-first and trust-led; families pay for human reassurance about an anxious situation. Keep a human in the loop on family-facing care moments and any incident.
- **Liability stays human.** A care incident needs a human accountable chain; agents draft and triage, humans decide and own.
- **Automation isn't free.** It shifts cash payroll → model spend (far cheaper, but real and subject to subscription/rate limits) — and **requires the product platform (`syahar-app`) to be built** so agents have a system to operate.
- **Approval gates remain.** Per company rule, budget (incl. model spend to run agents) needs CEO approval.

## 5. Action — agent-hire roadmap (replicate the marketing-pod model)
1. **Now:** marketing pod (live). 
2. **Phase 2:** Analytics/Data agent + Customer Success agent (replace the Data Engineer + CS hires).
3. **Phase 2–3:** Ops Coordinator agent (augments human coordinators — automates matching/scheduling/report compilation).
4. **Phase 3–4:** Finance agent (augments CFO — models/reporting) + Legal-research agent (augments Counsel).
5. **Ongoing:** Claude as the engineering force-multiplier — hold engineering headcount flat while output grows.

Each hire follows the proven pattern: define the agent, equip it with skills, report to its human lead, gate its run-budget on CEO approval.
