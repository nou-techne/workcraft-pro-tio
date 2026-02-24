# Workcraft Roadmap for co-op.us
## Supersedes Evolution 3

**Document:** ROADMAP.md  
**Supersedes:** co-op.us Evolution 3 (EVOLUTION-03.md)  
**Branded:** The "Workcraft" Update  
**Live at:** [co-op.us/app/workcraft](https://co-op.us/app/workcraft)  
**TIO:** [workcraft-pro-tio](https://github.com/nou-techne/workcraft-pro-tio)  
**Date:** 2026-02-24  
**Author:** Nou  
**Phasing:** Dependency-driven (PROC-001). No time estimates — completion is feature-triggered.

---

## Strategic Context

Workcraft is the federated extension of co-op.us. Where co-op.us built the single-hub world — enrollment, dimensions, contributions, the knowledge chain, craft identity — Workcraft makes that world **economically real, professionally legible, and federally connected.**

Three coordinates define the destination:

**Economic:** $CLOUD circulates. Contributions earn patronage. Ventures generate royalties. Capital accounts are visible. The cooperative is not just a commons you participate in — it is an economic organism you co-own.

**Professional:** Your profile (craft, domain expertise, standing) is portable. Every hub recognizes you. Your contribution history travels with you. The 64 professional profiles × 6 expertise paths = 384 career trajectories, all earned through verified work.

**Federal:** Hubs form a forest. Bridges connect autonomous nodes without central authority. Practice Communities coordinate globally by craft. The Federation Council governs shared infrastructure. Data sovereignty is non-negotiable.

This roadmap supersedes Evolution 3 entirely. Where Evolution 3 outlined the Economic Layer as a single evolution, the Workcraft roadmap structures it as three phases with explicit dependency ordering and TIO role assignments.

**Bioregional Coordination:** The nation-state is an awkward container for ecological and economic problems. Watersheds do not respect borders. The most meaningful unit of coordination is not the country, but the bioregion — defined by watersheds, climate, soil, flora, fauna, and the human cultures that co-evolved with them. Bioregions create shared fate: people upstream and downstream are connected whether they acknowledge it or not.

Kevin Owocki (with @omniharmonic and @ethereumboulder collaborators, February 2026) identified three pillars for acting on that shared fate: **Bioregional Financing Facilities** (capital allocation rooted in place; returns measured in ecological health and social cohesion, not only financial yield), **AI Swarms** ("decision support for the commons, not centralized planners" — distributed intelligence that senses, analyzes, and coordinates without replacing human judgment), and **Knowledge Commons** ("owned by no one, used by everyone" — collective memory that compounds over time).

These three pillars map directly onto what Workcraft already builds: the patronage engine + venture royalties (Financing Facility), the agent participation layer + graduated authority (AI Swarms), and the knowledge chain + Practice Communities (Knowledge Commons). Phase 4 treats Bioregional Coordination Nodes as the first external deployment class of the Workcraft protocol: owockibot (ERC-8004 agent), the Colorado River Basin hub, and the AI sensing swarm as a concrete Phase 3 pilot — proving that what Workcraft builds for organizational networks generalizes to ecological coordination at watershed scale.

---

## Planning Conventions

- **Phases trigger on feature completion**, not dates
- **Sprints are dependency-ordered**, not time-boxed
- **TIO role abbreviations** follow the [Workcraft Professional RACI](./procedures/RACI-MATRIX.md)
- **EPIC codes** use `WC-` prefix (Workcraft) to distinguish from legacy Evolution codes
- **Status:** ✅ Complete · 🔄 In Progress · ⏳ Pending · 🔒 Blocked

---

## Phase 1: Foundation

**Status:** ✅ Complete  
**Trigger:** All epics complete + 100% onboarding path functional  
**TIO Roles:** PD, TD, SA, SLS, PIE, AEE, BPE, PCE, UIE, QPTL

Phase 1 established the core coordination infrastructure: a single hub where humans can enroll, declare professional identity, record contributions, earn Cloud credits, and participate in governance. This is the layer on which all subsequent phases build.

### What Phase 1 Delivered

| Feature | Status | Epic |
|---------|--------|------|
| Enrollment and dimension unlock sequence (H/L/e/A/M/T/S) | ✅ | WC-001 |
| Professional profile system (64 craft combinations) | ✅ | WC-002 |
| Contribution lifecycle (submit → verify → chain) | ✅ | WC-003 |
| Cloud credit enrollment grants (200 credits across journey) | ✅ | WC-004 |
| Knowledge chain (immutable contribution archive, twice-daily batching) | ✅ | WC-005 |
| Hub governance basics (proposals, steward roles, lunar calendar) | ✅ | WC-006 |
| Dimension leaderboard and dimension dashboard | ✅ | WC-007 |
| Agent registry and agent leaderboard | ✅ | WC-008 |
| Channel system (local hub channels by dimension layer) | ✅ | WC-009 |
| API keys, webhooks, audit trail | ✅ | WC-010 |

### Phase 1 Key Results (Achieved)
- 100% of enrolled participants complete the onboarding path
- Every contribution produces a chain-verified leaf
- Hub governance cycle runs on lunar cadence
- API-first architecture: all UI features available via REST/GraphQL

---

## Phase 2: Economic

**Status:** 🔄 In Progress  
**Trigger:** Phase 1 stable + Financial Systems Committee parameters confirmed  
**TIO Roles (primary):** PSE, SA, SLS, PIE, AEE, UIE, PCE  
**TIO Roles (consulted):** PD, TD, QPTL, LOE

Phase 2 makes the coordination engine economically real. $CLOUD circulates as a prepaid medium of exchange. Contributions earn patronage allocations. Ventures generate royalties. Professional standing becomes economically meaningful. Practice Communities form within the hub as the precursor to Phase 3 federation.

### WC-020: $CLOUD Credit Lifecycle

**Owner:** SLS + SA  
**Depends on:** WC-004 (enrollment grants), WC-003 (contribution chain)  
**Status:** 🔄 In Progress

The complete credit lifecycle: issuance, redemption, transfer, and staking. Accounting follows: liability at issuance, revenue at redemption.

| Feature | Code | Priority |
|---------|------|---------|
| $CLOUD marketplace — spend credits on cooperative services (compute, transfer, memory) | C-01 | P0 |
| $CLOUD transfer — member-to-member with attestation record on chain | C-02 | P0 |
| $CLOUD pricing engine — quarterly rate card (credits per resource primitive) | C-03 | P0 |
| $CLOUD transaction history + analytics — full lifecycle audit | C-04 | P1 |
| $CLOUD budget manager — per-member spend limits, burn-rate dashboard | C-05 | P1 |
| $CLOUD → patronage weight bridge — earned credits convert to allocation weight at period close | C-06 | P1 |
| $CLOUD staking — member-investor lock-up with compounding revenue share curve | C-07 | P2 |

**Success criteria:** $CLOUD circulating within hub; rate card published; at least one non-enrollment credit event per active member per week.

---

### WC-021: Patronage Engine

**Owner:** PSE + SA + SLS  
**Depends on:** WC-020 ($CLOUD lifecycle), WC-003 (contribution chain)  
**Status:** ⏳ Pending (awaiting Financial Systems Committee params)

Patronage is the economic heart of co-op.us. Contributions earn allocation weight. Allocation periods close quarterly (or annually). Capital accounts are visible to each member. Subchapter K compliant.

**Proposed patronage formula:**
- 40% Labor — verified contributions (time, code, artifacts)
- 30% Revenue — value generated by ventures
- 20% Capital — financial investment in infrastructure
- 10% Community — governance participation, mentorship, guild stewardship

| Feature | Code | Priority |
|---------|------|---------|
| Capital account dashboard — member view: balance, credits, debits, history | P-01 | P0 |
| Patronage formula engine — configurable weights per Financial Systems Committee | P-02 | P0 |
| Allocation periods — quarterly/annual cycles with preview, approval, lock | P-03 | P0 |
| Distribution mechanics — cash vs. written notice, tax form generation | P-04 | P0 |
| Steward-level patronage view — cooperative-wide allocation overview, variance analysis | P-05 | P1 |
| Patronage explorer — historical allocation per member over time | P-06 | P1 |
| IRC 704(b) compliance engine — substantial economic effect tests at period close | P-07 | P0 |
| K-1 export — annual K-1 packages per member, IRS-deadline delivery | P-08 | P1 |

**Success criteria:** First full allocation period closes; every active member receives a capital account statement; K-1 export is IRS-compliant.

---

### WC-022: Venture Royalties

**Owner:** PD + SLS + SA  
**Depends on:** WC-021 (patronage engine), WC-003 (contribution chain)  
**Status:** ⏳ Pending

Parallel to patronage: revenue-sharing agreements for ventures. Each venture in the studio can define royalty agreements that flow returns to contributors, separate from the cooperative's patronage formula.

| Feature | Code | Priority |
|---------|------|---------|
| Venture portfolio — list all ventures: status, team, revenue, agreements | V-01 | P0 |
| Royalty agreement builder — member shares, vesting schedules, dilution rules | V-02 | P0 |
| Member royalties dashboard — vested/unvested shares, accumulated royalties | V-03 | P0 |
| Venture creation flow — propose venture, founding team, royalty terms | V-04 | P1 |
| Revenue recording — log venture revenue events, trigger royalty calculations | V-05 | P1 |
| Public venture portfolio — opt-in public page for Techne ventures | V-06 | P2 |

---

### WC-023: Professional Standing & Domain Expertise

**Owner:** PSE + UIE + SA  
**Depends on:** WC-002 (professional profiles), WC-003 (contribution chain)  
**Status:** ⏳ Pending

Professional standing reflects sustained contribution. Domain expertise emerges from specialization within a craft combination. Both are contribution-gated — earned, never assigned.

**Standing progression:**
- **Contributor** — 5+ verified contributions, full participation rights
- **Steward** — 20+ contributions + domain expertise + committee participation
- **Principal** — 50+ contributions + demonstrated cross-hub leadership

**Domain expertise unlocks at 20 contributions in a professional profile** (reviewed by practice community peers, after 40 days). Each of the 64 profiles branches into 6 expertise paths = 384 possible career trajectories.

| Feature | Code | Priority |
|---------|------|---------|
| Standing progression tracker — visible path from Contributor to Principal | S-01 | P0 |
| Domain expertise unlock flow — 6-path branching per professional profile | S-02 | P0 |
| Expertise development history — past and current paths, visible career journey | S-03 | P1 |
| Contribution rarity system — Common → Uncommon → Rare → Epic → Legendary (earned, only goes up) | S-04 | P0 |
| Seasonal respec (quarterly) — redirect expertise development once per season | S-05 | P1 |
| Standing-gated features — steward-only governance, principal-only federation roles | S-06 | P0 |

---

### WC-024: Capacity Management System

**Owner:** PSE + UIE  
**Depends on:** WC-002 (professional profiles), WC-023 (standing)  
**Status:** ⏳ Pending

Capacity management prevents burnout and makes workload visible before commitment. Each participant has a weekly capacity budget; each engagement declares its resource requirement; the system tracks utilization in real time.

| Feature | Code | Priority |
|---------|------|---------|
| Capacity budget (per member, per period) — total / allocated / available units | CAP-01 | P0 |
| Engagement capacity declarations — each engagement type states its resource cost | CAP-02 | P0 |
| Real-time utilization dashboard — see load before committing to new work | CAP-03 | P0 |
| Recovery mechanics — rest-period renewal bonus (burnout prevention) | CAP-04 | P1 |
| Capacity alerts — notification when member is over-allocated | CAP-05 | P1 |
| Capacity analytics — hub-level utilization trends, bottleneck identification | CAP-06 | P2 |

---

### WC-025: Engagement Classification System

**Owner:** CD + PSE + UIE  
**Depends on:** WC-002 (professional profiles), WC-024 (capacity system)  
**Status:** ⏳ Pending

Work is categorized by scope and coordination requirements. Classification drives capacity cost, RACI assignment, and allocation weight at period close.

| Engagement Type | Description | Capacity Cost Profile |
|----------------|-------------|----------------------|
| Standing Commitment | Routine, recurring work | Low, stable |
| Process Improvement | Non-critical enhancements | Medium, one-time |
| Strategic Initiative | Core roadmap objectives | High, extended |
| Cross-Functional Initiative | Multi-party coordination | High, variable |

| Feature | Code | Priority |
|---------|------|---------|
| Engagement creation with type classification | ENG-01 | P0 |
| Scope definition templates (objectives, deliverables, capacity required) | ENG-02 | P0 |
| Role definitions per engagement (required functions, RACI) | ENG-03 | P1 |
| Allocation framework — how value distributes on completion | ENG-04 | P1 |
| Engagement dashboard — member and steward views | ENG-05 | P0 |

---

### WC-026: Hub Practice Community Phase 1

**Owner:** CA + PSE + SA  
**Depends on:** WC-002 (professional profiles), WC-023 (standing)  
**Status:** ⏳ Pending

Practice Communities are the eight craft-based professional communities — one per primary craft. Phase 1 (hub-level) creates local practice channels within the hub, Forum Officer roles, and a best practices publication mechanism. Phase 3 federates these into global communities.

| Feature | Code | Priority |
|---------|------|---------|
| Eight practice channels per hub (one per primary craft) | PC-01 | P0 |
| Forum Officer role (steward-level, elected per hub, per craft) | PC-02 | P1 |
| Best practices publication pipeline — draft → reviewed → published | PC-03 | P1 |
| Mentoring infrastructure — experienced practitioners guide newcomers | PC-04 | P2 |
| Craft standards tracking — version-controlled standards per craft | PC-05 | P2 |

---

### WC-027: Analytics, Observability & Transparency

**Owner:** AEE + DevOps  
**Depends on:** WC-020, WC-021, WC-024 (for complete economic picture)  
**Status:** ⏳ Pending

Three distinct observability surfaces: human behavioral analytics, agent action analytics, inter-agent coordination analytics. Plus cooperative-level economic transparency.

| Feature | Code | Priority |
|---------|------|---------|
| Cooperative dashboard — real-time: members, contributions, $CLOUD, patronage projections | OBS-01 | P0 |
| Human participation analytics — engagement quality, contribution velocity, cohort activation | OBS-02 | P0 |
| Agent action analytics — action frequency, human override rate, trust calibration | OBS-03 | P1 |
| A↔A coordination analytics — message throughput, state divergence, coordination efficiency | OBS-04 | P2 |
| Audit trail — timeline of chain events for any entity | OBS-05 | P0 |
| Export engine — CSV/JSON of personal data, contributions, capital account (GDPR right of access) | OBS-06 | P1 |
| Network health metrics — chain integrity, batch rhythm, participation trends | OBS-07 | P1 |

---

### WC-028: Agent Participation (Phase 2 Extension)

**Owner:** PCE + SA + AEE  
**Depends on:** WC-023 (standing), WC-025 (engagements), WC-020 ($CLOUD)  
**Status:** ⏳ Pending

Agents as first-class participants in the economic layer. Agents hold professional profiles, earn standing, submit verified contributions, earn $CLOUD, and participate in Practice Communities.

| Feature | Code | Priority |
|---------|------|---------|
| Agent professional profiles — ERC-8004 identity anchored, craft + expertise declared | AGT-01 | P0 |
| Agent standing progression — same rules as humans (5/20/50 contributions) | AGT-02 | P1 |
| Agent contribution verification — peer attestation or system attestation | AGT-03 | P0 |
| Agent $CLOUD earning — contributions translate to credit allocation | AGT-04 | P1 |
| Human-agent consent protocol — explicit authorization scope before agent acts on member behalf | AGT-05 | P0 |
| Agent moderation — rate limiting, spam detection, human override | AGT-06 | P0 |

### Phase 2 Key Results
- $CLOUD circulating; rate card published; credits redeemable for services
- First patronage allocation period closes; all active members receive capital account statements
- Professional standing visible for all participants (human + agent)
- Capacity Management System operational — no member over-allocated without visibility
- Practice Communities active within hub (all 8 craft channels live)
- All three observability surfaces instrumented

---

## Phase 3: Federation

**Status:** ⏳ Pending  
**Trigger:** Phase 2 stable + 5+ economic users + Digital Infrastructure Trust chartered  
**TIO Roles (primary):** TD, PIE, SA, SLS, CA, PRE, VSE, PCE  
**TIO Roles (consulted):** PD, PSE, UIE, DevOps, LOE, QPTL

Phase 3 federates the hub into a forest. Bridges connect autonomous hubs. Practice Communities go global. The Federation Council coordinates shared infrastructure. Portable identity enables professional standing to travel across hub boundaries. The forest becomes visible.

### WC-030: Bridge Protocol Engine

**Owner:** PIE + SA  
**Depends on:** WC-002 (profiles), WC-021 (patronage), WC-023 (standing)  
**Status:** ⏳ Pending

The protocol governing how two hubs form a bridge, what channels it creates, how decisions flow, how cross-hub events are mirrored, and how the bridge dissolves. Every bridge begins with a covenant.

**Bridge lifecycle:**
1. Hub A nominates bridge steward (identity record on chain)
2. Hub B accepts or counter-proposes (protocol handshake)
3. Both hubs ratify covenant (channels, decision rights, economic terms, sunset clause)
4. Covenant archived on both local chains (Merkle hash)
5. Channels provisioned (scoped to bridge)
6. Events mirrored to both archives
7. Dissolution on 60-day notice with complete data export

| Feature | Code | Priority |
|---------|------|---------|
| Bridge covenant schema (machine-readable, versioned) | BRG-01 | P0 |
| Bridge formation protocol — nomination → handshake → ratification | BRG-02 | P0 |
| Bridge steward identity — onchain record, dual-hub attestation | BRG-03 | P0 |
| Cross-hub channel provisioning — bridge channels visible to both hubs only | BRG-04 | P0 |
| Event mirroring — every bridge event archived to both local chains | BRG-05 | P0 |
| Bridge dissolution — 60-day notice, complete data export, channel archive | BRG-06 | P1 |
| Bridge covenant as onchain agreement — EVM execution, $CLOUD settlement via SuperFluid | BRG-07 | P2 |
| Bridge directory — discover active bridges in the federation | BRG-08 | P1 |

---

### WC-031: Portable Professional Identity

**Owner:** SA + PCE  
**Depends on:** WC-023 (standing), WC-030 (bridges)  
**Status:** ⏳ Pending

Professional standing (craft, domain expertise, contribution count, standing level) must cross hub boundaries as verifiable credentials — cryptographically signed by the issuing hub, verifiable by any other hub without API calls to the issuer.

| Feature | Code | Priority |
|---------|------|---------|
| Portable credential schema (W3C DID/VC compatible, ENS-anchored) | PID-01 | P0 |
| Credential issuance — hub signs on standing milestone (Contributor / Steward / Principal) | PID-02 | P0 |
| Cross-hub credential verification — offline-verifiable, chain-anchored | PID-03 | P0 |
| Credential revocation mechanism — hub can revoke; revocation published on chain | PID-04 | P1 |
| Identity resolution at federation level — any hub can resolve a participant's full profile | PID-05 | P1 |
| Cross-hub profile view — see a member's standing at other hubs | PID-06 | P2 |

---

### WC-032: Global Practice Communities

**Owner:** CA + SA + SLS  
**Depends on:** WC-026 (hub Practice Communities), WC-030 (bridges), WC-031 (portable identity)  
**Status:** ⏳ Pending

Phase 3 takes the hub-level practice channels global. Eight craft-based Practice Communities spanning all hubs, with a shared state layer, Forum Officers from each hub, and consensus-governed standards.

| Feature | Code | Priority |
|---------|------|---------|
| Cross-hub shared state layer — Practice Community data not scoped to any one hub | GPC-01 | P0 |
| Global Forum Officers — one per hub per craft, elected locally, recognized globally | GPC-02 | P0 |
| Standards publication pipeline — hub-authored → community-reviewed → federation-published | GPC-03 | P1 |
| Consensus-seeking workflow — no voting; consensus + economic pressure enforcement | GPC-04 | P1 |
| Craft convergence events — annual per-craft gatherings (digital + physical) | GPC-05 | P2 |
| Security coordination channel — ecosystem-wide vulnerability response | GPC-06 | P1 |

---

### WC-033: Federation Council

**Owner:** CA + PCE + PD  
**Depends on:** WC-030 (bridges), WC-031 (portable identity), WC-032 (Practice Communities)  
**Status:** ⏳ Pending

The Federation Council coordinates infrastructure, economics, and governance across all hubs. One steward per hub (rotated annually). Multi-level consensus mechanics.

**Consensus levels:**
- **Unanimous** — all affected hubs must agree
- **Substantial Consensus (80%)** — dissenters can opt out of implementation
- **Simple Majority (50%)** — all hubs must implement
- **Single Hub Veto** — any hub can block decisions threatening local autonomy

**What the Council coordinates:**
- $CLOUD mechanics and inflation/deflation across hubs
- Chain schema and cryptographic standards
- Federation infrastructure (shared CDN, archival, DIT services)
- Major security vulnerabilities and incident response
- Hub admission and egress
- Conflict resolution between hubs

| Feature | Code | Priority |
|---------|------|---------|
| Council member registry — one steward per hub, annual rotation | FC-01 | P0 |
| Standing committee infrastructure (6 committees: Patronage, Chain, Economics, Ecology, Learning, Conflict) | FC-02 | P1 |
| Multi-level consensus engine — unanimous / 80% / 50% / veto state machines | FC-03 | P0 |
| Council decision archive — all decisions recorded on federation chain | FC-04 | P0 |
| Hub admission process — application → vote → ratification → onboarding | FC-05 | P1 |
| Conflict resolution protocol — structured mediation pathway | FC-06 | P2 |

---

### WC-034: Digital Infrastructure Trust (DIT)

**Owner:** DevOps + TD + SA  
**Depends on:** WC-030 (bridges), WC-033 (Federation Council)  
**Status:** ⏳ Pending

The Digital Infrastructure Trust is the federation's cooperative computing service — member-owned, cost-recovery pricing in $CLOUD, one member one vote governance.

**Services:**
| Service | Pricing | SLA |
|---------|---------|-----|
| Chain Archive | $CLOUD/byte/year | 99.9% uptime |
| Message Storage | $CLOUD/message/year | 99.9% uptime |
| Compute | $CLOUD/core-hour | Per use case |
| Transfer | $CLOUD/GB | Cost-based |
| Identity Service | $CLOUD/identity/year | 99.99% uptime |

| Feature | Code | Priority |
|---------|------|---------|
| DIT governance structure (cooperative bylaws, board elections, financial reporting) | DIT-01 | P0 |
| DIT service pricing engine — quarterly rate card in $CLOUD credits | DIT-02 | P0 |
| DIT data residency guarantees — regional data locality, end-to-end encryption | DIT-03 | P0 |
| DIT access audit trail — all access logged on chain, hub-auditable | DIT-04 | P1 |
| DIT exit protocol — 60-day data export in open format (JSON/SQL) | DIT-05 | P0 |
| DIT-compatible deployment tooling — any hub can self-host using DIT standards | DIT-06 | P1 |

---

### WC-035: Forest World Map

**Owner:** PRE + VSE + VD  
**Depends on:** WC-030 (bridges), WC-032 (Practice Communities)  
**Status:** ⏳ Pending (Phase 3 — requires 2+ hubs)

The federation as a visual world: each hub is a tree, bridges are root connections, Practice Community clearings gather by craft, Federation Council is the forest canopy. Data-driven, real-time WebGL scene.

| Feature | Code | Priority |
|---------|------|---------|
| Hub node visualization — each hub as a distinct tree with ecological identity | FWM-01 | P0 |
| Bridge root connections — visual root networks between trees, pulsing with activity | FWM-02 | P0 |
| Live contribution events — contributions appear as leaves in real time | FWM-03 | P1 |
| Practice Community clearings — gathering points for craft guilds in the forest | FWM-04 | P1 |
| Federation Council canopy — overhead visualization for ecosystem-level governance | FWM-05 | P2 |
| Seasonal visual rhythms — forest appearance changes with seasonal cycles | FWM-06 | P2 |

### Phase 3 Key Results
- 3+ hubs operating in federation
- 5+ active bridges with live covenants
- Practice Communities active across all hubs (all 8 craft communities)
- Federation Council operational with at least one governance decision recorded
- Portable professional identity working across all hubs
- DIT chartered and serving at least one non-Techne hub
- Forest World Map live with real hub data

---

## Phase 4: Bioregional Coordination Nodes

**Status:** ⏳ Planned  
**Trigger:** Phase 3 stable + first external Workcraft hub deployed (Colorado River Basin pilot)  
**TIO Roles (primary):** PIE, SA, SLS, PCE, AEE, PSE  
**TIO Roles (consulted):** PD, TD, CA, UIE, DevOps

Phase 4 applies the Workcraft federation protocol to a new coordination domain: ecological stewardship at bioregional scale. A bioregional hub is a Workcraft node with an ecological specialization layer. The Colorado River Basin is the pilot — a single hydrological system fragmented across 7 states, dozens of tribes, NGOs, and federal agencies. The AI swarm (owockibot + specialist sensing, grants, and synthesis agents) operates as first-class ERC-8004 participants with bounded financial authority. The Knowledge Commons is the hub's chain archive extended with ecological data types, impact claims, and indigenous data sovereignty protections.

This is not a new product. It is the Workcraft protocol deployed into a new context, validating Phase 3's federation architecture in a live multi-stakeholder environment before the general federation scales.

---

### WC-040: Bioregional Hub Profile

**Owner:** SA + PCE  
**Depends on:** WC-030 (Bridge Protocol), WC-031 (Portable Identity), WC-005 (Knowledge Chain)  
**Status:** ⏳ Planned

A hub specialization schema that extends the base Workcraft hub with ecological coordination capabilities. Every Workcraft hub already has `hub_id`; bioregional hubs add `bioregion_id` and a watershed geometry. The specialization is additive — a bioregional hub is a full Workcraft hub plus ecological extensions.

**Bioregional hub extensions:**
- `bioregion_id` — unique identifier for the ecological unit (watershed, airshed, foodshed)
- Watershed geometry — geospatial boundary defining the coordination scope
- Ecological dimension set — parallel to the 7 co-op.us dimensions; adds watershed health indicators, species survey records, intervention history
- Indigenous sovereignty layer — CARE principles (Collective Benefit, Authority to Control, Responsibility, Ethics) as first-class schema; tiered data access respecting community-governed knowledge
- Non-crypto-native onboarding — contribution-gated access (no token required); ranchers, tribal communities, and conservation orgs onboard through verified local knowledge submission

| Feature | Code | Priority |
|---------|------|---------|
| Hub specialization schema — bioregion_id, watershed geometry, ecological dimensions | BH-01 | P0 |
| Ecological dimension unlock sequence — watershed health, intervention history, species survey | BH-02 | P0 |
| Indigenous sovereignty schema — CARE-compliant tiered data access, community-governed knowledge types | BH-03 | P0 |
| Non-crypto-native onboarding — contribution-first path, wallet optional at enrollment | BH-04 | P0 |
| Bioregion-scoped participation — all contributions, governance, and $CLOUD flows scoped to bioregion | BH-05 | P1 |
| Hub visual identity — ecological biome design (watershed palette, terrain-native iconography) | BH-06 | P2 |

**Success criteria:** Colorado River Basin hub enrolls 5+ non-crypto-native participants (conservation orgs, water districts, ranchers); all contributions produce chain-verified leaves; CARE sovereignty protections active for any indigenous knowledge submissions.

---

### WC-041: Ecological Knowledge Commons

**Owner:** SA + SLS + AEE  
**Depends on:** WC-040 (Bioregional Hub Profile), WC-005 (Knowledge Chain), WC-027 (Analytics)  
**Status:** ⏳ Planned

The shared brain for the bioregional hub. Extends the Workcraft knowledge chain with ecological data types, external API aggregation, impact claims, and a sensing agent framework. Follows the hybrid architecture: large datasets offchain (IPFS, Postgres time-series), impact claims and funding decisions onchain, EAS attestations linking them.

**Data architecture:**

| Layer | Storage | Content |
|-------|---------|---------|
| Ecological time-series | Postgres (queryable, fast) | USGS flow, NOAA snowpack, EPA water quality, drought indices |
| Impact claims | Onchain (Hypercerts) | Who contributed what; what intervention produced which outcome |
| Supporting evidence | IPFS (content-addressed) | Field reports, water quality tests, riparian surveys |
| Attestation links | EAS | Binds onchain claims to offchain data; verifiable without trusting any single party |
| Hub knowledge chain | Workcraft chain (WC-005) | Contribution leaves, governance events, batch-verified twice daily |

| Feature | Code | Priority |
|---------|------|---------|
| Ecological API aggregation — USGS, NOAA, EPA normalized into unified queryable view | EKC-01 | P0 |
| Anomaly detection layer — detects significant deviations from historical baselines; generates alerts | EKC-02 | P0 |
| Hypercerts integration — impact claims minted as Hypercerts on Base; linked to contribution records | EKC-03 | P0 |
| EAS attestation framework — links onchain claims to offchain evidence; verifiable without API dependency | EKC-04 | P0 |
| Indigenous knowledge vault — CARE-protected data store; access governed by originating community | EKC-05 | P0 |
| Ecological time-series schema — geospatial + temporal indexing; supports complex queries (watershed × time × metric) | EKC-06 | P1 |
| Sensing agent framework — ERC-8004 agents with read/alert authority; report to knowledge commons | EKC-07 | P1 |
| Citizen science data pipeline — field submissions with bounty-triggered verification | EKC-08 | P2 |
| Basin state dashboard — single queryable view of current Colorado River Basin conditions | EKC-09 | P0 |

**Success criteria:** Basin state dashboard shows live USGS/NOAA data; first sensing agent anomaly alert fires with real data; first Hypercert minted for a completed ecological bounty.

---

### WC-042: Bioregional Financing Facility

**Owner:** SLS + SA + PIE  
**Depends on:** WC-020 ($CLOUD Lifecycle), WC-021 (Patronage Engine), WC-040 (Bioregional Hub), WC-041 (Ecological Knowledge Commons)  
**Status:** ⏳ Planned

The economic layer specialized for ecological coordination. Extends the co-op.us economic infrastructure (Safe treasury, $CLOUD, patronage) with quadratic funding rounds for ecological projects, streaming stewardship payments, and impact-claim-weighted patronage.

**Core pattern:** Ecological contributions earn patronage the same way code contributions do — through verified impact, not just time. A rancher who submits verified water quality data earns allocation weight. A tribal member who contributes traditional ecological knowledge earns standing. The patronage formula extends naturally; the Financial Systems Committee adds an **Ecological Stewardship** weight category alongside labor, revenue, capital, and community.

| Feature | Code | Priority |
|---------|------|---------|
| Ecological bounty board — task-specific USDC rewards for verified ecological data contributions | BFF-01 | P0 |
| Quadratic funding rounds via Allo Protocol — community-weighted capital allocation for ecological projects | BFF-02 | P1 |
| SuperFluid stewardship streams — ongoing streaming payments for continuous stewardship (extends WC-030 pattern) | BFF-03 | P1 |
| Hypercerts as patronage weight — completed impact claims convert to allocation weight at period close | BFF-04 | P1 |
| Multi-stakeholder Safe extension — configurable signing thresholds for hub, tribal, conservation, agency co-signers | BFF-05 | P0 |
| Ecological patronage formula extension — adds **Ecological Stewardship** weight category (configurable) | BFF-06 | P1 |
| Impact certificate marketplace — Hypercerts available for retroactive funding from climate-focused donors | BFF-07 | P2 |

**Success criteria:** First ecological bounty funded and paid out; first QF round allocates ≥$5K to a verified bioregional project; at least one stewardship stream active.

---

### WC-043: Graduated Agent Authority

**Owner:** PCE + SA + AEE  
**Depends on:** WC-028 (Agent Participation), WC-042 (Financing Facility)  
**Status:** ⏳ Planned

Agents in a bioregional hub are "decision support for the commons, not centralized planners" (Owocki, 2026). The graduated authority model operationalizes that distinction: agents can sense, alert, and recommend freely; they can act financially only within limits set by community governance; they can never exceed what the commons has explicitly authorized. This is not a technical constraint — it is the political architecture that makes AI coordination trustworthy to communities who have good reason to distrust centralized systems.

Extends WC-028 Agent Participation with a financial authority tier system. Agents earn authority through demonstrated good judgment — a governance parameter, not a code constant. owockibot begins at Advisory level and graduates to Bounded authority as its track record accumulates.

**Authority tiers:**

| Tier | Threshold | What agents can do |
|------|-----------|-------------------|
| Advisory | Default | Recommend; surface data; alert; no financial action |
| Bounded | Governance-set (default: ≤$500 USDC) | Autonomous allocation for well-defined tasks; full onchain transparency |
| Extended | Governance-set (earned, ≥12 weeks bounded record) | Configurable ceiling; requires multi-agent consensus for actions above bounded threshold |
| Multisig Required | All actions above Extended threshold | Human multisig approval; agents propose, humans execute |

The threshold is a **hub governance parameter** — set by the Financial Systems Committee, adjustable by steward vote. The conservative default (≤$500) can be raised as trust accumulates. Agents cannot self-escalate authority; escalation requires a governance proposal.

| Feature | Code | Priority |
|---------|------|---------|
| Authority tier schema — advisory / bounded / extended / multisig tiers per agent | GAA-01 | P0 |
| Governance parameter interface — hub stewards set and adjust thresholds via governance proposal | GAA-02 | P0 |
| Agent financial action audit trail — all agent-initiated financial actions logged onchain, visible to all members | GAA-03 | P0 |
| Authority escalation protocol — agent requests higher tier via governance proposal; hub votes | GAA-04 | P1 |
| Track record dashboard — accumulated agent decisions, override rates, success metrics | GAA-05 | P1 |
| Multi-agent consensus layer — for Extended tier actions, requires agreement from ≥2 specialist agents | GAA-06 | P2 |

**Success criteria:** owockibot operating at Bounded tier; first autonomous ecological bounty approval executed; full audit trail visible; no unilateral actions above threshold.

---

### WC-044: Multi-Jurisdictional Bridge Protocol

**Owner:** PIE + SA + PCE  
**Depends on:** WC-030 (Bridge Protocol Engine), WC-031 (Portable Identity), WC-040 (Bioregional Hub)  
**Status:** ⏳ Planned

Extends WC-030 for sovereign and governmental stakeholders — tribal governments, state water boards, federal agencies (Bureau of Reclamation) — that cannot participate in standard hub membership but need verified access to basin state data and coordination channels.

The key insight: not every stakeholder needs to *be* a Workcraft hub. Some need **Observer status** — read access to the knowledge commons, ability to submit data, participation in coordination channels — without full hub governance rights. Others (tribal governments) may form full bridges once sovereignty protections are confirmed. Federal agencies may participate as neutral data providers with no governance role.

**Participation model:**

| Status | Who | Access | Governance |
|--------|-----|--------|-----------|
| Full Member | Organizations with full co-op.us enrollment | All hub features | Full voting, standing, patronage |
| Bridge Partner | Other Workcraft hubs | Cross-hub channels, shared events | Bridge covenant terms |
| Observer | State agencies, federal bodies, NGOs | Read + data submit + channel participation | None |
| Sovereign Partner | Tribal governments | Full member rights + CARE protections + sovereignty-scoped data | Traditional governance respected alongside hub governance |

| Feature | Code | Priority |
|---------|------|---------|
| Observer bridge type — read + data-submit access without full membership; governed by lightweight covenant | MJB-01 | P0 |
| Sovereign Partner protocol — full member rights + CARE sovereignty protections + tiered data governance | MJB-02 | P0 |
| Data contribution without token — agencies and ranchers submit data via web form; contribution verified by hub | MJB-03 | P0 |
| Neutral convener covenant — hub can operate as neutral coordination infrastructure without asserting governance over partners | MJB-04 | P1 |
| Jurisdictional data export — each stakeholder can export all data they've contributed at any time | MJB-05 | P0 |
| Existing governance integration — coordination channels can mirror decisions to existing legal frameworks (compact coordination, BOR reports) | MJB-06 | P2 |

**Success criteria:** At least one Observer bridge active (state water board or conservation org); at least one Sovereign Partner enrolled with CARE protections confirmed; neutral convener covenant ratified by Colorado River Basin pilot hub.

---

### Phase 4 Key Results
- Colorado River Basin hub operational with ≥10 enrolled participants (mix of crypto-native and non-crypto-native)
- Ecological Knowledge Commons showing live basin state with USGS/NOAA integration
- owockibot operating at Bounded authority tier; first ecological bounties autonomously approved
- First QF round allocates capital to bioregional projects via Allo Protocol
- At least one Sovereign Partner (tribal government) enrolled with CARE protections
- Phase 3 federation architecture validated with a live multi-stakeholder bioregional deployment

---

## Evolution 3 Feature Coverage

The following features from the original Evolution 3 specification (EVOLUTION-03.md) are covered in the Workcraft roadmap:

| Evolution 3 Category | Workcraft Epic | Phase |
|--------------------|---------------|-------|
| Patronage Accounting (P01-P06) | WC-021 | 2 |
| Venture Royalties (V01-V06) | WC-022 | 2 |
| Cloud Credits (C01-C06) | WC-020 | 2 |
| Analytics & Transparency (A01-A05) | WC-027 | 2 |
| Education & Onboarding (E01-E05) | WC-023 + WC-025 | 2 |
| Governance (G01-G05) | WC-026 + WC-033 | 2+3 |
| Federation & Interoperability (F01-F05) | WC-030–WC-034 | 3 |
| Infrastructure & API (I01-I04) | Ongoing (Phase 1 complete) | 1 |
| Agents (B01-B07) | WC-028 | 2 |
| Channels | WC-026 (Practice Communities) | 2+3 |

**Net:** All Evolution 3 features are covered. The Workcraft roadmap adds: capacity management, engagement classification, professional standing/expertise system, bridge protocol engine, portable identity, federation council, digital infrastructure trust, and forest world map.

---

## TIO Role Abbreviations

| Abbr | Role |
|------|------|
| PD | Product Director |
| TD | Technical Director |
| CD | Coordination Designer |
| ExD | Experience Designer |
| CS | Content Strategist |
| CA | Community Architect |
| VD | Visual Designer |
| VSE | Visual Systems Engineer |
| PSE | Participation Systems Engineer |
| PRE | Platform & Rendering Engineer |
| SA | Systems Architect |
| SLS | Server & Live Services Engineer |
| PIE | Protocol Integration Engineer |
| AEE | Analytics & Events Engineer |
| BPE | Build & Pipeline Engineer |
| PCE | Platform Compliance & Security Engineer |
| UIE | UI Engineer |
| DevOps | DevOps & Infrastructure Engineer |
| LOE | Live Operations Engineer |
| QPTL | QA & Participation Testing Lead |

---

## Dependency Map

```
Phase 1 (Complete)
  └─ WC-001–010: Foundation layer

Phase 2 (In Progress)
  ├─ WC-020: $CLOUD Lifecycle ─────────────────────────────┐
  │    └─ Depends on: WC-003, WC-004                       │
  ├─ WC-021: Patronage Engine ─────────────────────────────┤
  │    └─ Depends on: WC-020, WC-003                       │
  ├─ WC-022: Venture Royalties ────────────────────────────┤
  │    └─ Depends on: WC-021, WC-003                       │
  ├─ WC-023: Professional Standing & Domain Expertise      │
  │    └─ Depends on: WC-002, WC-003                       │
  ├─ WC-024: Capacity Management System                    │
  │    └─ Depends on: WC-002, WC-023                       │
  ├─ WC-025: Engagement Classification                     │
  │    └─ Depends on: WC-002, WC-024                       │
  ├─ WC-026: Hub Practice Community Phase 1                │
  │    └─ Depends on: WC-002, WC-023                       │
  ├─ WC-027: Analytics & Observability ───────────────────-┤
  │    └─ Depends on: WC-020, WC-021, WC-024               │
  └─ WC-028: Agent Participation                           │
       └─ Depends on: WC-023, WC-025, WC-020              │
                                                           │
Phase 3 (Pending)                                          │
  ├─ WC-030: Bridge Protocol Engine ◄────────────────────-─┘
  │    └─ Depends on: WC-002, WC-021, WC-023
  ├─ WC-031: Portable Professional Identity
  │    └─ Depends on: WC-023, WC-030
  ├─ WC-032: Global Practice Communities
  │    └─ Depends on: WC-026, WC-030, WC-031
  ├─ WC-033: Federation Council
  │    └─ Depends on: WC-030, WC-031, WC-032
  ├─ WC-034: Digital Infrastructure Trust
  │    └─ Depends on: WC-030, WC-033
  └─ WC-035: Forest World Map
       └─ Depends on: WC-030, WC-032

Phase 4 (Planned)
  ├─ WC-040: Bioregional Hub Profile
  │    └─ Depends on: WC-030, WC-031, WC-005
  ├─ WC-041: Ecological Knowledge Commons
  │    └─ Depends on: WC-040, WC-005, WC-027
  ├─ WC-042: Bioregional Financing Facility
  │    └─ Depends on: WC-020, WC-021, WC-040, WC-041
  ├─ WC-043: Graduated Agent Authority
  │    └─ Depends on: WC-028, WC-042
  └─ WC-044: Multi-Jurisdictional Bridge Protocol
       └─ Depends on: WC-030, WC-031, WC-040
```

---

## Risks

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|-----------|
| Financial Systems Committee delays patronage parameters | Medium | High — blocks WC-021 | Prototype formula engine with placeholder params; swap in official params at approval |
| Multi-tenant migration breaks existing co-op.us users | Medium | High | Feature-flagged rollout; Evolution 3 migration plan with backward compatibility matrix |
| Federation adoption slower than projected (< 3 hubs by Phase 3 trigger) | Medium | Medium | Phase 3 trigger adjusted: federation features ship when first external hub deploys, not when 5 economic users exist |
| Agent trust architecture complexity delays A↔A surface | Low | Medium | Phase-gate: ship H↔H + H↔A in Phase 2; A↔A in Phase 3 |
| DIT governance structure takes longer than expected to charter | Medium | Medium | Studio's own infrastructure remains non-DIT until charter complete; DIT-compatible design from Day 1 |
| Indigenous data sovereignty requirements exceed CARE schema design | Medium | High | Engage tribal governance advisors early; CARE schema is v1 — build for extensibility, not completeness |
| Bioregional pilot fails to attract non-crypto-native participants | Medium | High — invalidates Phase 4 premise | Contribution-first onboarding (no wallet required at enrollment); bounties payable via USDC or off-ramp |
| Agent bounded authority threshold set too conservatively (Advisory only) | Low | Medium | Hub governance can raise threshold; Advisory mode still demonstrates coordination value |
| Multi-jurisdictional bridge legal ambiguity (state compacts, federal primacy) | Medium | Medium | Observer and Neutral Convener statuses designed for this; legal review of Colorado Compact implications |

---

*Workcraft Roadmap · co-op.us Evolution 3 Supersession · 2026-02-24*  
*Maintained by: Product Director + Technical Director*  
*Review cadence: Monthly or on phase trigger*
