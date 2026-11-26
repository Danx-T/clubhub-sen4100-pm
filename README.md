# ClubHub (`CLUBHUB-001`) — Project Management & Milestone Deliverables

**Course:** SEN4100 — Software Project Management (Haliç University)  
**Sponsor / Instructor:** Asst. Prof. M. Fatih Mintaş  
**Project:** ClubHub: Survey, Membership and Participation Management Platform for Student Clubs

## Team
| Member | Student ID | Code | Role |
|---|---|---|---|
| Danyal TUNÇ | 23091390009 | `DT` | Project Manager / Developer & Tester |
| Devran DUMAN | 22092090021 | `DD` | Business Analyst / Developer & Tester |
| Muhammed Taha ŞEN | 22092090030 | `MT` | Lead Developer / Tester |

## Project Baseline Summary
- **Scope:** 6 MVP modules (User Auth & 3-Role RBAC, Club Management, Membership, Surveys, Events & Attendance, Reports with UTF-8 BOM CSV export) decomposed into **6 Control Accounts**, **14 Deliverables**, and **17 Work Packages (`1.1.1`–`6.2.1`)**.
- **Schedule & Effort Baseline:** 13-week semester (`65 working days`), **180 person-hours BAC** (`60h` per member, `88 Story Points`, `0 TRY` direct cash budget) plus an **18h (10%)** PM-managed contingency reserve (`198h` ceiling).
- **Lifecycle:** Scrum with 2-week sprints (`Sprints 1–4` in Weeks 5–12, preceded by Initiation Weeks 1–4 and followed by Closure Week 13).

## Repository Deliverables (Milestones 1–3)
| Deliverable | File | Milestone | Status |
|---|---|---|---|
| Milestone 1 Initiation Package (Charter, Stakeholders, Scope, TELOS) | `MILESTONE1.pdf` | M1 (Wk 4) | Delivered |
| Milestone 2 Planning Baseline (WBS, PERT/CPM, Gantt, COCOMO, Risks) | `MILESTONE2.pdf` | M2 (Wk 7) | Delivered |
| Earned Value Management (EVM) Performance Tracking Report | `EVM_Performance_Report.pdf` | M3 (Wk 13) | Tracked via WBS `1.2.1` |
| Comprehensive Final Project Documentation (IEEE Format) | `Final_Project_Documentation_IEEE.pdf` | M3 (Wk 13) | Tracked via WBS `6.2.1` |
| Live Team Oral Defense Slides | `Oral_Defense_Slides.pptx` | M3 (Wk 13) | Tracked via WBS `6.2.1` |
| Oral Defense Walkthrough, Q&A Prep & Retrospective | `Oral_Defense_Walkthrough_and_Retrospective.pdf` | M3 (Wk 13) | Tracked via WBS `6.2.1` |
| Software Configuration Management (SCM) Audit Report | `SCM_Audit_Report.pdf` | M3 (Wk 13) | Tracked via WBS `1.2.1` |

## Branching & SCM Workflow (Aligned with M2 §6 Table 6.1)
- `main`: Protected release branch holding baseline and final approved milestone packages.
- `dev`: Integration branch receiving verified Milestone 3 deliverables before final release cutover (`dev` → `main`).
- `docs/<wbs-id>-<slug>`: Short-lived WBS-prefixed working branches (e.g., `docs/1.2.1-evm-report`, `docs/6.2.1-ieee-final-report`, `docs/6.2.1-oral-defense`, `docs/1.2.1-scm-audit`) merged into `dev` via Pull Requests with merge commits preserved (`--no-ff` / GitHub merge commit).

## Issue & Backlog Tracking Note
All **17 WBS Work Packages (`1.1.1`–`6.2.1`)** are provisioned in **GitHub Issues** and **GitHub Milestones (`M1–M3`)** using labels for `owner` (`DT`/`DD`/`MT`), `critical-path`, sprint/period, and linked Risk IDs (`R-01`–`R-10`).  
*Tooling note:* Programmatic **GitHub Projects v2** board automation requires the `project` / `read:project` OAuth scope, which is not present on the local Git Credential Manager token (`gist, repo, workflow` scopes only); therefore, GitHub Issues, Milestones, and Labels provide the active REST-managed tracking layer.
