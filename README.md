# Workcraft Professional TIO

*Technology and Information Office — Workcraft Enterprise (Professional) Edition*

**Forked from:** [nou-techne/tio](https://github.com/nou-techne/tio)  
**Companion:** [nou-techne/game-studio-tio](https://github.com/nou-techne/game-studio-tio) (cultural/game vocabulary edition)  
**Principal Project:** Workcraft × co-op.us — Evolution 3 and beyond  
**Studio Size:** 20 roles  
**Date:** 2026-02-24  

---

## What This Is

The **Workcraft Professional TIO** is a 20-role Technology and Information Office structured for building Workcraft Enterprise — the distributed coordination framework that merges with co-op.us as Evolution 3.

This edition uses **professional/enterprise vocabulary** throughout. The cultural/game track (archetypes, guilds, specializations, ecology metaphors) exists in the companion [game-studio-tio](https://github.com/nou-techne/game-studio-tio) — both track the same underlying coordination system, expressed in different languages.

---

## The Principal Project

**Workcraft** is a distributed operating system for cooperative organizational networks. It extends co-op.us from a single hub into a peer-to-peer federation:

- **Single hub → Forest:** Each organization is an autonomous node; together they form a federation
- **Profiles → Portable identity:** Professional standing and credentials travel across hub boundaries
- **Coordination → Protocol:** H↔H, H↔A, and A↔A interaction surfaces built from the same API
- **Patronage → Economic flows:** $CLOUD credits, contribution verification, period-close allocation

**Three phases:**

| Phase | Name | Trigger | Status |
|-------|------|---------|--------|
| 1 | Foundation | Epics complete + 100% onboarding | ✅ Complete |
| 2 | Economic | Phase 1 stable + Financial Systems Committee params | 🔄 In Progress |
| 3 | Federation | Phase 2 stable + 5+ economic users + DIT | ⏳ Planned |

→ Full roadmap: [ROADMAP.md](./ROADMAP.md)  
→ Live at: [co-op.us/app/workcraft](https://co-op.us/app/workcraft)

---

## Seven-Layer Stack → Workcraft

| Layer | Pattern | TIO Role | Workcraft Domain |
|-------|---------|----------|-----------------|
| 1 | Identity | Systems Architect | Participant entity schema, hub structure, bridge covenant schema |
| 2 | State | Server & Live Services | $CLOUD balances, capital accounts, hub state, leaderboards |
| 3 | Relationship | Protocol Integration Engineer | Bridge protocol, platform SDK integrations, API federation |
| 4 | Event | Analytics & Events Engineer | Coordination events, 3-surface telemetry (H↔H, H↔A, A↔A) |
| 5 | Flow | Build & Pipeline Engineer | Contribution lifecycle, period close, asset and build pipeline |
| 6 | Constraint | Platform Compliance & Security | Agent trust policies, GDPR, hub governance rules |
| 7 | View | UI Engineer + Platform & Rendering Engineer | Dual-track UX (pro + cultural), WebGL forest world map |

---

## The 20-Role Roster

### Leadership
| # | Role | Scope |
|---|------|-------|
| 1 | [Product Director](./roles/00-product-director.md) | Vision, roadmap, stakeholder communication, Evolution 3 |
| 2 | [Technical Director](./roles/00-technical-director.md) | Architecture, dependency ordering, technical leadership |

### Design
| # | Role | Scope |
|---|------|-------|
| 3 | [Coordination Designer](./roles/01-coordination-designer.md) | Participation mechanics, governance design, capacity system |
| 4 | [Experience Designer](./roles/02-experience-designer.md) | User journeys, onboarding flows, dimension progression |
| 5 | [Content Strategist](./roles/03-content-strategist.md) | Vocabulary, documentation, in-app text, API content |
| 6 | [Community Architect](./roles/04-community-architect.md) | Practice Community design, bridge covenant structure, guild governance |

### Visual
| # | Role | Scope |
|---|------|-------|
| 7 | [Visual Designer](./roles/05-visual-designer.md) | SVG/WebGL assets, dark-first, hub visual identities, no animation |
| 8 | [Visual Systems Engineer](./roles/06-visual-systems-engineer.md) | Art-to-engine pipeline, shader effects, forest map visual binding |

### Engineering — Core
| # | Role | Scope |
|---|------|-------|
| 9 | [Participation Systems Engineer](./roles/07-participation-systems-engineer.md) | Coordination loop, capacity management, governance state machines |
| 10 | [Platform & Rendering Engineer](./roles/08-platform-rendering-engineer.md) | WebGL pipeline, forest world map, GPU performance |

### Engineering — Stack (Layers 1–7)
| # | Role | Layer | Scope |
|---|------|-------|-------|
| 11 | [Systems Architect](./roles/09-systems-architect.md) | 1 | Entity schema, multi-tenant, portable credentials, bridge schema |
| 12 | [Server & Live Services Engineer](./roles/10-server-live-services.md) | 2 | $CLOUD lifecycle, hub state, Practice Community storage |
| 13 | [Protocol Integration Engineer](./roles/11-protocol-integration-engineer.md) | 3 | Bridge protocol engine, platform SDKs, shared feature surface |
| 14 | [Analytics & Events Engineer](./roles/12-analytics-events-engineer.md) | 4 | 3-surface event schemas, agent health dashboards |
| 15 | [Build & Pipeline Engineer](./roles/13-build-pipeline-engineer.md) | 5 | CI/CD, asset pipeline, Evolution 3 migration tooling |
| 16 | [Platform Compliance & Security Engineer](./roles/14-platform-compliance-security.md) | 6 | Agent trust (ERC-8004), GDPR, federation governance compliance |
| 17 | [UI Engineer](./roles/15-ui-engineer.md) | 7 | Dual-track UX, capacity dashboard, federation UI |

### Engineering — Operations
| # | Role | Scope |
|---|------|-------|
| 18 | [DevOps & Infrastructure Engineer](./roles/16-devops-infrastructure.md) | DIT-compatible deployment, monitoring, environments |

### Operations & Quality
| # | Role | Scope |
|---|------|-------|
| 19 | [Live Operations Engineer](./roles/17-live-operations-engineer.md) | Post-launch, guild infrastructure, $CLOUD economy monitoring |
| 20 | [QA & Participation Testing Lead](./roles/qa-participation-testing-lead.md) | Cross-layer quality, participation loop testing, compliance verification |

---

## Key Documents

- **[ROADMAP.md](./ROADMAP.md)** — Complete Workcraft roadmap; supersedes co-op.us Evolution 3
- **[GAPS_AND_OPPORTUNITIES.md](./GAPS_AND_OPPORTUNITIES.md)** — Living analysis; inherits from [game-studio-tio v1](https://github.com/nou-techne/game-studio-tio/blob/main/GAPS_AND_OPPORTUNITIES.md) and [v2](https://github.com/nou-techne/game-studio-tio/blob/main/GAPS_AND_OPPORTUNITIES_v2_WORKCRAFT.md)
- **[ADAPTATION_NOTES.md](./ADAPTATION_NOTES.md)** — What changed from the source TIO and why
- **[procedures/DEPENDENCY_DRIVEN_PLANNING.md](./procedures/DEPENDENCY_DRIVEN_PLANNING.md)** — Planning methodology (retained from source TIO)
- **[procedures/RACI-MATRIX.md](./procedures/RACI-MATRIX.md)** — 20-role coordination matrix

---

## Related Repositories

| Repo | Purpose |
|------|---------|
| [nou-techne/tio](https://github.com/nou-techne/tio) | Source TIO (Techne cooperative context) |
| [nou-techne/game-studio-tio](https://github.com/nou-techne/game-studio-tio) | Cultural/game vocabulary TIO edition |
| [Roots-Trust-LCA/co-op.us](https://github.com/Roots-Trust-LCA/co-op.us) | Workcraft implementation |
| [Roots-Trust-LCA/workcraft](https://github.com/Roots-Trust-LCA/workcraft) | Workcraft specification |
| [nou-techne/habitat](https://github.com/nou-techne/habitat) | Patronage accounting infrastructure |

---

*Workcraft Professional TIO · 2026 · Forked from Techne TIO*
