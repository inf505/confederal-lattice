# Handoff — County-Confederal Design Corpus

**Written**: 2026-11-03 (updated 2026-11-04)
**State**: v1.2 tagged, 23 corpus files (+ `AGENTS.md`), 46 tracked issues, 3 open CRITICAL items scoped
**Purpose**: Context for the next session. Read this first, then `README.md`, then **`critical-path.md`**.

> **START HERE NEXT SESSION**: `critical-path.md`. The design is complete; validation is not. Three open `CRITICAL` issues (OI-14, OI-27, OI-28) are scoped there with method, data, pass/fail thresholds, and design levers. Run them in the order OI-27 → OI-14 → OI-28. Do not start with OI-28.

---

## 1. What This Is

A complete design for dismantling the U.S. federal state and replacing it with a county-based confederation. Written as a thought experiment: one dictatorial act, then vanish.

It began as 22 "taboo" items that neither major party will touch (`solutions.md`) and grew into a 20-file constitutional architecture plus one analysis file.

**Core principles**: subsidiarity, exit over voice, voluntary coordination, no permanent center.

**Not**: a forecast, a democratic transition plan, or a validated system. Numbers are illustrative.

---

## 2. Current State

| Item               | Value                                                                                    |
| ------------------ | ---------------------------------------------------------------------------------------- |
| **Version**        | v1.2 (2026-11-03)                                                                        |
| **Files**          | 23 `.md` (20 design/meta + `critical-path.md` + `corruption-analysis.md` + this handoff) |
| **Change sets**    | 12 (CS1–CS12; CS12 is documentation only)                                                |
| **Tracked issues** | 46 (OI-01 … OI-46)                                                                       |
| **Status mix**     | 2 MITIGATED · 30 OPEN · 6 DEFERRED · 8 RESOLVED                                          |
| **Severity**       | 5 CRITICAL · 13 HIGH · 21 MEDIUM · 7 DECISIONS                                           |
| **Git**            | `main`, clean, tags `v1.0` / `v1.1` / `v1.2`                                             |

### Tags

| Tag    | Commit    | Meaning                           |
| ------ | --------- | --------------------------------- |
| `v1.0` | `4fbd4de` | Frozen baseline: 20 files, CS1–10 |
| `v1.1` | `44aad01` | Post-freeze design work (CS11)    |
| `v1.2` | `9d614b6` | External reviews integrated       |

Recover any baseline with `git checkout v1.0` (or `v1.1`, `v1.2`).

---

## 3. What Happened This Session

### Freeze lifted

The design freeze (imposed before external evaluation) was removed. Design changes are now permitted. `README.md` version line reflects this.

### CS11 — Post-Freeze Design Work

| ID   | Change                                                                                                                                                                       |
| ---- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| D-1  | Small-county consolidation offer (<10,000 pop or 2-yr unstaffed → largest contiguous county in-state; joint consolidation allowed; commission consent + majority referendum) |
| D-2  | Contiguous-only consolidation                                                                                                                                                |
| D-3  | Automatic marshal on 72-hour refusal (Art VI / Art II §2.1 / Art II §6)                                                                                                      |
| D-4  | Sheriff bond formula: 10% of prior-year LVT, min $50k, max $500k                                                                                                             |
| D-5  | `3,143` → "all counties" generalization across 10 files                                                                                                                      |
| D-6  | Registry: added `DEF-01`, renamed `OPS-01` to "Civic Operations"                                                                                                             |
| D-7  | Consistency pass (marshal scope, commission consent, status arithmetic)                                                                                                      |
| D-8  | Nuclear surviving-majority fallback + proof-of-life protocol (resolves OI-24)                                                                                                |
| D-9  | Voluntary equity-driven transition levy                                                                                                                                      |
| D-10 | Phased opt-in debt swap for retail holders                                                                                                                                   |

### External reviews integrated (3)

| Review                | Problem                                            | Resolution                                                                                          |
| --------------------- | -------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **#1 Enforcement**    | Rogue sheriff + physical resistance vacuum         | Economic containment (primary) + compact expulsion (secondary) — decentralized, no central force    |
| **#2 Nuclear**        | 50-governor unanimity = decapitation vulnerability | Surviving-majority fallback, crypto proof-of-life (30-min), denominator shift 50→N, monthly testing |
| **#3 Capital flight** | Haircut + levy + legal-tender repeal = flight      | Voluntary equity levy (D-9) + retail debt swap (D-10); new OI-46 tracks the residual risk           |

### Residual Nuclear Vulnerabilities (post-CS11 D-8)

These remain **by design** — the trade-off is fragile deterrent > capturable deterrent.

| Vulnerability                        | Description                                                                                                                    | Design Position                                                                         |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| **Total C3 loss = paralysis**        | EMP/cyber/physical comms destruction → no proof-of-life pings return → denominator cannot be established → no launch authority | Accepted. No central command = no single point of capture.                              |
| **Launch-on-actual-detonation only** | Trigger requires _confirmed nuclear strike_, not launch-on-warning. First strike lands unanswered.                             | Intentional — prevents accidental launch from false positives.                          |
| **Small survivor cabal**             | 2/3 of _survivors_ (not 2/3 of 50). If only 5 governors reachable, 4 can launch.                                               | Accepted — prevents single holdout from blocking retaliation.                           |
| **Protocol atrophy**                 | Monthly testing required; if neglected, protocol fails in crisis.                                                              | Operational risk, not design flaw. Council maintains quarterly verified-alive registry. |
| **Spoofed proof-of-life**            | Adversary spoofs crypto pings to inflate denominator or fake alive governors.                                                  | Crypto auth spec in `defense-lattice.md`; not yet stress-tested.                        |
| **Civil war / fragmented authority** | Two factions claim legitimate governors. Who controls ping infrastructure?                                                     | Unresolved — falls to political resolution, not protocol.                               |
| **Conventional decapitation**        | Adversary uses conventional hypersonics to decapitate; no nuclear detonation → no trigger → no nuclear response.               | Intentional gap. Nuclear deterrent only covers nuclear attack.                          |

### External review items NOT adopted

- Mandatory administrative pooling / inverse-LVT SWF seeding (breaks no-redistribution firewall)
- **Automatic** economic quarantine (would create a central enforcement trigger) — decentralized version adopted instead
- Staggered legal-tender phase-out / federal Stability Corps (would create a permanent transition state)

### Issues resolved this session

- **OI-05** — AG recall aligned to electing body (county commission majority)
- **OI-09** — surcharge holdout accepted as designed
- **OI-24** — nuclear fallback with proof-of-life
- **OI-40** — AG selection (county commissions)

### New files

- `corruption-analysis.md` — layer-by-layer corruption surface map with friction at each level

---

## 4. Key Design Decisions (with rationale)

| Decision                                | Rationale                                                                                                                             |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| **Friction over force**                 | Bad actors face escalating cost (bond, recall, audit, containment, expulsion) rather than gunpoint enforcement. No capturable center. |
| **No central enforcement**              | A federal enforcement apparatus _will_ be captured. Accept occasional pariah counties as the cost.                                    |
| **Economic containment before marshal** | Uses existing border/compact authority; no central trigger; no armed escalation.                                                      |
| **Surviving-majority nuclear fallback** | Prevents adversary decapitation from disabling deterrence; keeps 2/3 threshold (not unanimous survivors).                             |
| **Voluntary transition mechanisms**     | Equity levy and debt swap are opt-in, use existing county instruments, reduce capital-flight incentives without new federal programs. |
| **Consolidation is voluntary**          | Commission consent + majority referendum in each county; no forced merger.                                                            |

---

## 5. Working Rules (carry forward)

1. **Verify every claim against current text with grep before editing.** External evaluators have a high error rate (stale snapshots + fabricated citations). Treat all citations as unverified.
2. **Canonical sources**: `constitution.md` = rules; `README.md` = navigation/registry; `changelog.md` = history; `open-issues.md` = open work.
3. **Log every change** in `changelog.md` (append to CS11 or start CS12).
4. **New problems go to `open-issues.md`** — check there first; if listed, sharpen the test; if not, add a new OI.
5. **Historical filenames in `changelog.md` are intentional** — never "fix" them.
6. **Edit tool re-aligns markdown table padding** — use unique in-cell substrings or prose anchors as match targets, never full padded rows.
7. **Commit per batch** with a descriptive message; tag at meaningful milestones.

---

## 6. Where To Go Next

### Critical path (highest value) — **detailed in `critical-path.md`**

The three open `CRITICAL` issues are now scoped as runnable tests. `critical-path.md` contains, for each: what the corpus claims, what is unproven, the method, the data, the pass/fail threshold, candidate findings, and the design levers available if the test fails.

| Order | ID        | Issue                                                                         | Decisive check                                                                                   |
| ----- | --------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| **1** | **OI-27** | Debt math — $60T+ claims vs ~$5T assets                                       | Does the ~0.5%-of-LVT assessment fund a $19–22T Trust-note coupon at 1%? (Likely no — see §2.5.) |
| **2** | **OI-14** | County capacity — can small counties staff sheriff/court/mutual/LVT/cyber?    | Derive a minimum-viable-county population floor; test the 10 smallest counties; test refusal.    |
| **3** | **OI-28** | Transition feasibility — 5 years, 12M personnel, 150k prisoners, all charters | Build the dependency graph; find the first slip (Stand-Up is internally circular — see §3.5).    |

**Run OI-27 first.** It sets the fiscal envelope the other two depend on. Running OI-28 first produces a plan with no funding and no staffing assumptions.

**Adjacent, run in parallel**: OI-03 (reimbursement vs 15% cap) and OI-46 (capital flight) share the OI-27 spreadsheets. OI-29 (prisoner transfer) runs inside OI-28.

### Open HIGH items (9)

OI-10 (state revenue volatility), OI-15 (county insolvency), OI-16 (LVT assessment capture), OI-18 (currency oracle), OI-21 ($60M budget realism), OI-23 (war powers speed / "defensive"), OI-29 (prisoner transfer capacity), OI-35 (re-centralization risk), OI-37 (macroeconomic stabilization)

### Open MEDIUM items (18)

OI-06, OI-07, OI-08, OI-11, OI-12, OI-13, OI-17, OI-19, OI-20, OI-22, OI-25, OI-26, OI-31, OI-32, OI-33, OI-34, OI-36, OI-38

### MITIGATED (untested)

- **OI-03** — minimum-standard reimbursement vs 15% cap (numeric budget test pending)
- **OI-46** — capital flight during transition (model 20–30% outflow in Years 0–2)

### Deferred decisions (6)

OI-39, OI-41, OI-42, OI-43, OI-44, OI-45

### Suggested next actions

1. **Open `critical-path.md`** — it is the work plan for the three open CRITICAL items.
2. **Run OI-27 first** — build the debt settlement spreadsheet. The decisive check is the Trust-note coupon: does ~0.5% of LVT fund $19–22T at 1%? (`critical-path.md` §2.3, Step 2).
3. **Run OI-14** — derive the minimum-viable-county floor, then test the 10 smallest real counties (52–570 pop range found earlier) and the consolidation-refusal case.
4. **Run OI-28** — dependency graph first, then throughput arithmetic; identify the first milestone to slip.
5. **Continue external review loop** — load corpus into NotebookLM, ask for contradictions; verify every citation before editing.

---

## 7. File Map

### Core

| File                     | Role                                               |
| ------------------------ | -------------------------------------------------- |
| `README.md`              | Master index, subsystem registry, glossary, status |
| `constitution.md`        | 9 Articles — canonical rules                       |
| `changelog.md`           | Change Sets 1–12 + optional add-ons + anchor index |
| `open-issues.md`         | 46 tracked issues with severity/owner/test         |
| `critical-path.md`       | Validation work plan for OI-14 / OI-27 / OI-28     |
| `corruption-analysis.md` | Corruption surface map + friction by layer         |

### Design files (by subsystem ID)

| ID            | File                                                         |
| ------------- | ------------------------------------------------------------ |
| CON-01        | `constitution.md`                                            |
| JUD-01        | `judicial-system.md`                                         |
| LAW-01        | `law-enforcement.md`                                         |
| RTS-01        | `civil-liberties.md`                                         |
| HLT-01        | `healthcare.md`                                              |
| INF-01        | `infrastructure.md`                                          |
| BDR-01        | `border-immigration.md`                                      |
| DEF-01        | `defense-lattice.md`                                         |
| TRN-01…ENR-01 | `domestic-policy.md` §1–§9                                   |
| FRN-01…EMS-01 | `vestigial-functions.md` §1–§4                               |
| DEB-01        | `debt-obligations.md`                                        |
| AST-01        | `asset-transfer.md`                                          |
| PER-01        | `personnel-transition.md`                                    |
| OPS-01        | `civic-operations.md`                                        |
| —             | `public-finance.md` (money, taxation, pensions, term limits) |
| —             | `solutions.md` (the 22 taboos + solutions)                   |
| —             | `federal-remnant.md` (224 people)                            |

---

## 8. Verification Commands

```bash
# State
git --no-pager log --oneline --decorate -n 5
git --no-pager tag -n
git --no-optional-locks status --short --branch

# Consistency checks
grep -rn "3,143" --include=*.md .          # should be zero
grep -rn "~225" --include=*.md .           # only changelog history
grep -rn "Change Sets 1–" --include=*.md . # counters should read 1–12
grep -c "^| \*\*OI-" open-issues.md        # should be 46

# Cross-reference integrity
grep -rn "remaining-systems\|low-priority-systems\|continuity-and-operations\|system-gaps\|items\.md\|edits\.md" --include=*.md . | grep -v changelog
```

---

## 9. Known Quirks

- **`changelog.md` historical filenames** are intentional (pre-CS8 names). Do not "fix."
- **Severity table includes resolved items** in their severity buckets (OI-01, OI-24, OI-30 are listed despite being resolved). The status mix is authoritative for totals.
- **`DECISIONS` row** in the severity table covers OI-39–45 regardless of status.
- **Numbers are illustrative** — LVT rates, budgets, debt arithmetic are sketches (OI-27 tracks reconciliation).
- **`corruption-analysis.md`** is analysis, not a subsystem — it has no registry ID.

---

## 10. The Design in One Sentence

> Push all authority to counties, keep the state as a thin coordination layer, reduce the federal government to a mailbox and a mint, make bad behavior expensive rather than illegal, and let the designer vanish so there is no center to capture.

---

_End of handoff. Start with `README.md`, then `open-issues.md` §I for the current queue._
