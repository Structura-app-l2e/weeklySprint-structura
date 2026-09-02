# STRUCTURA

# OWNER / CLIENT — OWNER & INVESTOR PORTAL

## PRE-BACKLOG PRODUCT & ENGINEERING BLUEPRINT

**Document purpose:** Establish the agreed product, User Experience, engineering, financial, security, construction-domain, governance, and architectural baseline from which the Structura Owner / Client Product Backlog and detailed WBS (Work Breakdown Structure) will later be derived.

**Primary scope:** Owner / Client — Owner & Investor Portal

**Status:** Pre-Backlog Blueprint
**Product stage:** Existing PoC (Proof of Concept) → Defined Future-State Product Concept
**Important boundary:** This document does **not** create Product Backlog items, Sprint Backlog items, user stories, story points, engineering tasks, subtasks, or a detailed WBS (Work Breakdown Structure).

---

<a id="table-of-contents"></a>

# Table of Contents

> **Navigation tip:** Use the links below to jump to any major section. At the end of every major section, use **Back to Table of Contents** or the **Previous / Next** links.

- [1. Executive Summary](#section-1)
- [2. Scope](#section-2)
- [3. Current-State Owner Experience](#section-3)
- [4. Functional Status Matrix](#section-4)
- [5. Current User Journey](#section-5)
- [6. Current Problems and Friction](#section-6)
- [7. Guest-First Onboarding Proposal](#section-7)
- [8. BMONI Integration Assessment](#section-8)
- [9. Future-State Owner Experience](#section-9)
- [10. Current-to-Future Gap Analysis](#section-10)
- [11. Security and Authorization Model](#section-11)
- [12. Financial / Escrow Architecture Concept](#section-12)
- [13. 7-Track Governance Mapping](#section-13)
- [14. Proposed Repository Architecture](#section-14)
- [15. Cross-Track Dependency Map](#section-15)
- [16. Risk Register](#section-16)
- [17. Assumptions and Unknowns](#section-17)
- [18. Pre-Backlog Capability Inventory](#section-18)
- [19. Readiness Gate](#section-19)
- [20. Final Product Flow Summary](#section-20)
- [Blueprint Conclusion](#section-21)

---

<a id="section-1"></a>

# 1. Executive Summary

Structura currently exists as a visually developed construction-management PoC (Proof of Concept) that presents different project stakeholders with role-specific portals.

The detailed scope of this blueprint is the:

> **Owner / Client — Owner & Investor Portal**

The current Owner experience already demonstrates several valuable concepts:

* project overview;
* project-budget visibility;
* escrow-related controls;
* BOQ (Bill of Quantities) visibility;
* 360° 3D (Three-Dimensional) construction visualization;
* BIM (Building Information Modeling) concepts;
* SITREP (Situation Report) monitoring;
* site-log recording;
* Owner-to-Project-Director communication;
* quick navigation;
* browser-based export;
* AI (Artificial Intelligence)-labelled functions.

However, the current PoC (Proof of Concept) is primarily a **demonstration of experience and product intent**.

Many interfaces appear to represent sophisticated capabilities whose underlying:

* persistence;
* authentication;
* authorization;
* business logic;
* transaction processing;
* auditability;
* AI (Artificial Intelligence) processing;
* and external integrations

have not yet been fully verified.

The central engineering transformation required is therefore not simply:

> **“Add more screens.”**

It is:

> **Turn currently separated screens, actions, and demonstrations into one connected, secure, evidence-based project decision system.**

The future Owner experience is organized around six responsibilities:

> **SEE → UNDERSTAND → DECIDE → COMMUNICATE → TRANSACT → RECORD & AUDIT**

These responsibilities create a coherent product model in which the Owner can:

* see what is physically happening;
* understand the construction and financial meaning;
* make controlled decisions;
* communicate in project context;
* perform legitimate BMONI-supported financial actions;
* and reconstruct the complete history afterward.

This analysis is deliberately being completed **before** Product Backlog creation because backlog items should be derived from verified gaps and agreed architecture, not directly from visible buttons or assumptions.

**Navigation:** [↑ Back to Table of Contents](#table-of-contents) · [Next: 2. Scope →](#section-2)

---

<a id="section-2"></a>

# 2. Scope

## 2.1 Primary Scope

This blueprint analyses in detail:

# **Owner / Client — Owner & Investor Portal**

This includes:

* entry experience;
* Owner Command Desk;
* BOQ (Bill of Quantities) & Escrow Payouts;
* 360° Turnkey 3D (Three-Dimensional) Model;
* Executive SITREPs (Situation Reports);
* Owner Quick Tools;
* Direct Line communication;
* Export;
* AI (Artificial Intelligence) Director;
* project decisions;
* financial authorization;
* future BMONI integration;
* audit and traceability.

---

## 2.2 Context-Only Portals

Structura also currently presents:

* Senior Project Director Hub
* Prime General Contractor Station
* Independent Structural QA/QC (Quality Assurance / Quality Control) Portal

These remain part of the overall Structura system context.

They are intentionally **not analysed deeply** in this blueprint.

**Navigation:** [← Previous: 1. Executive Summary](#section-1) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 3. Current-State Owner Experience →](#section-3)

---

<a id="section-3"></a>

# 3. Current-State Owner Experience

## 3.1 Role Selection

The current first screen presents the four stakeholder portals and substantial information regarding:

* role;
* authority;
* modules;
* boundaries;
* responsibilities.

The Owner enters through:

> **Authenticate as Owner / Client**

### Verified behaviour

Clicking the control successfully opens the Owner Command Desk.

### Important distinction

The wording suggests authentication, but no actual:

* username;
* password;
* identity verification;
* session validation;
* role verification

was observed.

Therefore:

> **Navigation is verified. Authentication is not.**

---

# 3.2 Owner Command Desk

The Owner Command Desk serves as the central Owner dashboard.

Visible project information includes:

* Total Project Budget
* Escrow Balance
* Construction Progress
* Post-Handover Value

Other visible sections include:

* Live Escrow Milestone
* Change-Order approval area
* Live Site Feed
* Direct Line: Lead Project Director
* Owner Quick Tools

Primary navigation includes:

* Owner Command Desk
* BOQ (Bill of Quantities) & Escrow Payouts
* 360° Turnkey 3D (Three-Dimensional) Model
* Executive SITREPs (Situation Reports)
* AI (Artificial Intelligence) Director
* Export
* Exit / Switch Role

A Light / Night visual control is also present.

---

# 3.3 BOQ (Bill of Quantities) & Escrow Payouts

This screen presents:

* project-phase information;
* escrow status;
* inspection certificates;
* contractual payment information;
* cost allocations;
* BOQ (Bill of Quantities) variance information;
* category filters;
* escrow-release control.

One important action was tested:

> **Approve Escrow Release ($245,000)**

### Observed response

> **Disbursement Approved & Released**

The visible application state changed.

What has **not** been verified is whether:

* actual money moved;
* a database changed;
* the transaction persisted;
* another party received funds;
* a financial provider was called;
* an audit entry was generated.

---

# 3.4 360° Turnkey 3D (Three-Dimensional) Model

Navigation into the 3D (Three-Dimensional) model is functional.

The interface exposes concepts including:

* Finished Turnkey
* Proposed BIM (Building Information Modeling)
* camera control;
* rotation;
* lighting;
* storey isolation;
* exploded floors;
* model layers;
* wireframe;
* cinematic fly-around;
* snapshots;
* material specifications;
* interior layouts;
* architectural lighting;
* MEP (Mechanical, Electrical and Plumbing);
* microgrid-related information.

The page is therefore a substantial visual workspace.

However, not every individual control has yet been systematically tested.

---

# 3.5 Executive SITREPs (Situation Reports)

This page presents project monitoring and reporting information including:

* site activity;
* photo evidence;
* material information;
* QA/QC (Quality Assurance / Quality Control);
* periodic monitoring;
* site logbook;
* published reports;
* EVM (Earned Value Management);
* work-package information;
* quality milestones;
* cost/trade variance;
* Owner decisions.

Two important actions were tested.

### Record Site Log

Clicking the control opens a modal titled:

> **Record Site Logbook Entry**

The modal includes fields such as:

* cadence;
* weather;
* temperature;
* site headcount;
* period spend;
* trade/crew distribution;
* accomplished tasks;
* materials delivered and inspected.

The modal opens successfully.

Saving and persisting the entry has not yet been verified.

---

### Generate AI Weekly SITREP

When clicked:

* the button visually depresses;
* it returns to normal;
* no modal appears;
* no report appears;
* no navigation occurs;
* no visible error appears.

Therefore this is currently:

> **User Interface only / No observed functional outcome**

---

# 3.6 Owner Quick Tools

Two shortcuts were tested.

### Latest SITREP

Navigates successfully to its referenced SITREP (Situation Report) area.

### BOQ Audit Trail

Navigates successfully to its BOQ (Bill of Quantities) / audit-related destination.

Both are confirmed working navigation shortcuts.

---

# 3.7 Direct Line Communication

The Owner can enter a message and submit it.

The message appears immediately in the conversation thread with a recent timestamp.

This confirms a functional User Interface interaction.

It does **not** prove:

* server persistence;
* delivery to another user;
* notification;
* read status;
* synchronization between devices.

---

# 3.8 Export

Clicking Export opens browser Print Preview.

The observed dashboard rendered into multiple printable pages.

Therefore the current Export feature is a verified browser/system action.

It has not yet been established as a structured server-generated reporting or audit-export system.

---

# 3.9 AI (Artificial Intelligence) Director

The AI (Artificial Intelligence) Director is visible.

Its detailed behaviour has not yet been tested.

---

# 3.10 Exit / Switch Role

The control is visible.

Its exact behaviour remains unverified.

**Navigation:** [← Previous: 2. Scope](#section-2) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 4. Functional Status Matrix →](#section-4)

---

<a id="section-4"></a>

# 4. Functional Status Matrix

| Capability                                        | Current Status               | Evidence                                                    |
| ------------------------------------------------- | ---------------------------- | ----------------------------------------------------------- |
| Enter Owner / Client portal                       | **Functional**               | Opens Owner Command Desk                                    |
| Actual authentication                             | **Backend Unverified**       | No credential or identity flow observed                     |
| Owner Command Desk                                | **Functional**               | Dashboard renders and navigation works                      |
| BOQ (Bill of Quantities) screen                   | **Functional**               | Page navigation confirmed                                   |
| Approve Escrow Release                            | **Partially Functional**     | Visible state changes; real financial settlement unverified |
| BOQ (Bill of Quantities) filters                  | **Not Yet Tested**           | Controls visible                                            |
| 360° 3D (Three-Dimensional) Model                 | **Functional**               | Page navigation confirmed                                   |
| Individual 3D (Three-Dimensional) controls        | **Not Yet Tested**           | Controls visible                                            |
| BIM (Building Information Modeling) relationships | **Backend Unverified**       | Interface concept visible                                   |
| Executive SITREPs (Situation Reports)             | **Functional**               | Screen navigation confirmed                                 |
| Record Site Log modal                             | **Functional**               | Modal opens                                                 |
| Save Site Log                                     | **Not Yet Tested**           | Persistence unverified                                      |
| Generate AI Weekly SITREP                         | **User Interface Only**      | Visual press only                                           |
| Direct Line message submission                    | **Backend Unverified**       | Message appears; server delivery unknown                    |
| Latest SITREP shortcut                            | **Functional**               | Navigation verified                                         |
| BOQ Audit Trail shortcut                          | **Functional**               | Navigation verified                                         |
| Export                                            | **Functional**               | Browser Print Preview opens                                 |
| AI (Artificial Intelligence) Director             | **Not Yet Tested**           | Visible control                                             |
| Light / Night toggle                              | **Not Yet Tested**           | Visible                                                     |
| Exit / Switch Role                                | **Not Yet Tested**           | Visible                                                     |
| BMONI integration                                 | **Not Present / Unverified** | No observed BMONI-backed financial flow                     |
| Real transaction state                            | **Backend Unverified**       | Interface currently jumps to released state                 |
| Persistent audit system                           | **Backend Unverified**       | Audit interface exists but backend not verified             |

**Navigation:** [← Previous: 3. Current-State Owner Experience](#section-3) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 5. Current User Journey →](#section-5)

---

<a id="section-5"></a>

# 5. Current User Journey

The current Owner journey is approximately:

```text
STRUCTURA
   ↓
Role Selection
   ↓
Authenticate as Owner / Client
   ↓
OWNER COMMAND DESK
   │
   ├── BOQ & Escrow
   │      ↓
   │   Review financial information
   │      ↓
   │   Approve Escrow Release
   │      ↓
   │   “Disbursement Approved & Released”
   │
   ├── 360° Turnkey 3D Model
   │      ↓
   │   Inspect visual project information
   │
   ├── Executive SITREPs
   │      │
   │      ├── Record Site Log
   │      │      ↓
   │      │   Modal opens
   │      │
   │      └── Generate AI Weekly SITREP
   │             ↓
   │          No visible outcome
   │
   ├── Direct Line
   │      ↓
   │   Send message
   │      ↓
   │   Message appears
   │
   ├── Latest SITREP
   │
   ├── BOQ Audit Trail
   │
   └── Export
          ↓
       Print Preview
```

The current experience already demonstrates a coherent Owner concept.

Its largest limitation is that the **visible experience is ahead of the verified system architecture underneath it**.

**Navigation:** [← Previous: 4. Functional Status Matrix](#section-4) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 6. Current Problems and Friction →](#section-6)

---

<a id="section-6"></a>

# 6. Current Problems and Friction

## 6.1 Information density

The opening experience communicates too many concepts simultaneously.

The visitor sees:

* roles;
* modules;
* boundaries;
* responsibilities;
* project information;
* authentication-style actions

before understanding the core value of Structura.

---

## 6.2 Onboarding overload

The user is asked to understand Structura's organizational structure before experiencing the product.

The current journey begins closer to:

> **Understand the system → select role → explore**

rather than:

> **Experience value → explore → identify yourself when needed**

---

## 6.3 Authentication timing

The current entry says:

> **Authenticate as Owner / Client**

but actual authentication has not been verified.

Navigation and authentication are therefore conceptually mixed together.

---

## 6.4 Incomplete interactions

Some controls are functional while others primarily represent future intent.

The clearest example is:

> **Generate AI Weekly SITREP**

which currently provides only visual feedback.

---

## 6.5 Financial-state ambiguity

The current financial action jumps directly from:

> **Approve Escrow Release**

to:

> **Disbursement Approved & Released**

This visually collapses several potentially distinct states:

* construction approval;
* financial approval;
* authorization;
* transaction submission;
* processing;
* settlement.

---

## 6.6 Backend uncertainty

Several current interactions work in the browser but have unverified:

* persistence;
* synchronization;
* database state;
* server-side processing.

---

## 6.7 Feedback gaps

A user performing a major action should eventually be able to understand:

* what happened;
* whether it succeeded;
* whether it is still processing;
* whether additional action is required.

The current Proof of Concept does not consistently establish this distinction.

**Navigation:** [← Previous: 5. Current User Journey](#section-5) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 7. Guest-First Onboarding Proposal →](#section-7)

---

<a id="section-7"></a>

# 7. Guest-First Onboarding Proposal

## Core Principle

# **Experience value before authentication.**

Structura should not force the visitor to identify themselves before demonstrating what the product does.

---

# 7.1 Guest Experience

The public experience should use demonstration data only.

A visitor could explore:

* sample Owner Command Desk;
* sample project overview;
* sample BOQ (Bill of Quantities);
* sample SITREP (Situation Report);
* 3D (Three-Dimensional) model;
* example project progress;
* example financial milestone.

No real project data should be accessible.

---

# 7.2 Swipe / Slide Introduction

A short sequence could introduce the product concept.

### Slide 1 — SEE

> See your project without being everywhere.

Visual focus:

3D (Three-Dimensional) project / site evidence.

### Slide 2 — UNDERSTAND

> Understand progress, cost and quality.

Visual focus:

BOQ (Bill of Quantities), progress, reporting.

### Slide 3 — DECIDE

> Turn project evidence into informed decisions.

Visual focus:

milestones and approvals.

### Slide 4 — STAY CONNECTED

> Keep project communication and accountability visible.

Visual focus:

SITREP (Situation Report), Direct Line, audit history.

### Final choice

**Explore Demo**

or

**Access My Project**

---

# 7.3 Protected Actions

Authentication should be triggered by accessing real or sensitive information, such as:

* actual project data;
* real BOQ (Bill of Quantities);
* financial information;
* project communication;
* official site logs;
* project modification.

---

# 7.4 Financial Authorization Triggers

Additional authorization should be required for high-consequence actions, such as:

* escrow approval;
* actual payment authorization;
* changing payment destination;
* transaction signing;
* withdrawal;
* wallet/security changes.

---

# 7.5 Returning User Flow

A returning authorized Owner should normally bypass the introductory tour.

```text
Returning Owner
      ↓
Recognized / Authenticated
      ↓
Authorized Project
      ↓
Owner Command Desk
```

The product tour should remain optionally accessible.

**Navigation:** [← Previous: 6. Current Problems and Friction](#section-6) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 8. BMONI Integration Assessment →](#section-8)

---

<a id="section-8"></a>

# 8. BMONI Integration Assessment

## 8.1 What BMONI Provides

BMONI provides financial infrastructure including:

* financial user creation;
* smart wallets;
* KYC (Know Your Customer);
* financial rails;
* wallet balances;
* funding;
* money movement;
* transaction proposals;
* transaction signing;
* regional banking rails;
* withdrawals;
* transaction/event information.

BMONI should **not** be interpreted as providing Structura's construction milestone logic.

Structura remains responsible for answering:

> **Why should this payment happen?**

BMONI can support:

> **How does the authorized financial movement happen?**

---

# 8.2 BMONI Lifecycle

The financial lifecycle is:

```text
User
 ↓
Wallet
 ↓
KYC (Know Your Customer)
 ↓
Rail
 ↓
Fund
 ↓
Move Money
```

This means the Owner cannot realistically jump directly from:

> “Approve”

to:

> “Money moved”

without prerequisite financial readiness.

---

# 8.3 Current Structura Technology Compatibility

The current Structura structure indicates a browser-oriented TypeScript/TSX application using technologies such as Vite.

The supplied BMONI packages include Flutter-specific components.

Therefore:

### Flutter SDK (Software Development Kit)

Not directly compatible with the current web application.

### `bkey_uikit`

Flutter User Interface library.

Not directly required for current Structura web integration.

### `bmoni_embedded_wallets_cards`

Flutter-specific wallet components.

Not directly compatible with the existing browser application.

### BMONI REST API (Representational State Transfer Application Programming Interface)

This is the most appropriate integration surface for the existing Structura web architecture.

The recommended boundary is:

```text
Structura Browser
       ↓
Structura Back-end
       ↓
BMONI REST API
(Representational State Transfer
Application Programming Interface)
```

Sensitive BMONI partner credentials should not be embedded inside the public browser application.

---

# 8.4 Wallet Requirements

A real financial architecture must determine:

* which person owns or controls the wallet;
* whether a wallet represents an Owner, project, payment facility, or another financial entity;
* how wallet readiness is represented;
* how signing authority is controlled.

These decisions remain unresolved.

---

# 8.5 KYC (Know Your Customer)

BMONI financial use may require user identity verification before financial rails and money movement become available.

This onboarding should appear **only when relevant to financial activity**.

A user exploring a 3D (Three-Dimensional) model should not be forced into KYC (Know Your Customer).

---

# 8.6 Transaction Signing

Transaction signing is different from normal Structura authentication.

Structura authentication proves:

> **Who is this user?**

Financial signing proves:

> **Is this financial transaction properly authorized?**

The two boundaries should remain separate.

---

# 8.7 Minimum Meaningful Competition Integration

A meaningful competition demonstration should involve actual BMONI sandbox interaction.

Conceptually:

```text
Owner
 ↓
Structura Milestone / Financial Screen
 ↓
Structura Back-end
 ↓
Real BMONI Sandbox Request
 ↓
BMONI Wallet / Transaction Proposal
 ↓
Actual BMONI Transaction State
 ↓
Structura displays returned state
```

A stronger demonstration would also consume BMONI transaction events/webhooks and reflect actual:

* processing;
* completion;
* failure

inside Structura.

Merely displaying a BMONI logo would not constitute meaningful integration.

**Navigation:** [← Previous: 7. Guest-First Onboarding Proposal](#section-7) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 9. Future-State Owner Experience →](#section-9)

---

<a id="section-9"></a>

# 9. Future-State Owner Experience

The future Owner product is organized around six responsibilities.

# SEE

The Owner needs to answer:

> **What is happening?**

Capabilities include:

* live project information;
* project-health overview;
* 3D (Three-Dimensional) visualization;
* BIM (Building Information Modeling);
* site evidence;
* material lifecycle.

---

# UNDERSTAND

The Owner needs to answer:

> **What does this information mean?**

Capabilities include:

* BOQ (Bill of Quantities);
* project progress;
* SITREPs (Situation Reports);
* EVM (Earned Value Management);
* cost variance;
* quality information;
* certification status.

---

# DECIDE

The Owner needs to answer:

> **What requires my authority?**

Capabilities include:

* milestone decisions;
* change orders;
* financial approvals;
* escrow authorization;
* clarification requests.

---

# COMMUNICATE

The Owner needs to answer:

> **Who needs information or clarification?**

Capabilities include:

* contextual Direct Line communication;
* structured clarification requests;
* notifications.

---

# TRANSACT

The Owner needs to answer:

> **What authorized financial action should actually occur?**

Capabilities include:

* BMONI financial readiness;
* financial authorization;
* transaction proposal;
* transaction signing;
* transaction submission;
* transaction-state synchronization.

---

# RECORD & AUDIT

The Owner needs to answer:

> **What happened, who did it, and why?**

Capabilities include:

* decision history;
* transaction history;
* audit trail;
* reports;
* structured export.

**Navigation:** [← Previous: 8. BMONI Integration Assessment](#section-8) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 10. Current-to-Future Gap Analysis →](#section-10)

---

<a id="section-10"></a>

# 10. Current-to-Future Gap Analysis

| Capability                | CURRENT                            | GAP                                         | TARGET                                      |
| ------------------------- | ---------------------------------- | ------------------------------------------- | ------------------------------------------- |
| Entry                     | Dense role-first experience        | High cognitive load                         | Guest-first discovery                       |
| Authentication            | Navigation labelled authentication | No verified identity system                 | Real authenticated sessions                 |
| Role access               | User selects Owner                 | Role not verified                           | Project membership + role authorization     |
| Owner Command Desk        | Dashboard values                   | Data sources unverified                     | Connected decision-oriented command centre  |
| Project progress          | Percentage shown                   | Source unclear                              | Evidence-backed progress                    |
| BOQ (Bill of Quantities)  | Ledger presented                   | Domain persistence unverified               | Structured BOQ cost lifecycle               |
| Quality                   | Certificates visible               | Relationships unclear                       | Quality-gated milestone eligibility         |
| Milestones                | Represented visually               | Lifecycle unclear                           | Persistent evidence-backed lifecycle        |
| Escrow approval           | Immediate visible release          | Approval and payment conflated              | Multi-stage approval + transaction          |
| BMONI                     | No verified integration            | No real financial infrastructure connection | Server-side BMONI integration               |
| Transaction status        | Immediate released state           | No asynchronous lifecycle                   | Submitted / Processing / Completed / Failed |
| 3D (Three-Dimensional)    | Visual model                       | Data linkage unverified                     | BIM-linked project intelligence             |
| SITREP (Situation Report) | Reporting screen                   | AI generation absent                        | Data-backed report workflow                 |
| AI Weekly SITREP          | UI button only                     | No output                                   | Reviewable AI-generated draft               |
| Site Log                  | Modal works                        | Persistence unverified                      | Persistent site records                     |
| Messaging                 | Message appears                    | Backend unknown                             | Persistent contextual messaging             |
| Notifications             | Not verified                       | No event mechanism                          | Event-driven notifications                  |
| Audit Trail               | Shortcut exists                    | Backend audit unverified                    | Persistent event history                    |
| Export                    | Browser print                      | Not structured                              | Print + report + audit export               |
| Security                  | Access boundaries unclear          | High risk                                   | Layered security model                      |
| Testing                   | Manual observation                 | Automated coverage unknown                  | Multi-layer testing                         |
| Governance                | 7 tracks defined                   | Operational rules incomplete                | Risk-based multi-track review               |

**Navigation:** [← Previous: 9. Future-State Owner Experience](#section-9) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 11. Security and Authorization Model →](#section-11)

---

<a id="section-11"></a>

# 11. Security and Authorization Model

The future system should use progressively stronger trust levels.

## Level 0 — Guest Access

Can:

* explore Structura;
* view demonstration content;
* inspect sample model;
* view sample reports.

Cannot:

* access real project data;
* communicate with real project participants;
* view real financial information;
* perform project actions.

---

## Level 1 — Authenticated Access

The system verifies:

> **Who is this person?**

The user now has an identity and session.

---

## Level 2 — Project Membership

The system verifies:

> **Does this person belong to this project?**

---

## Level 3 — Role-Based Access

The system verifies:

> **Is this person actually authorized to act as Owner / Client?**

---

## Level 4 — Elevated Action Authorization

Required for consequential non-financial actions such as:

* milestone approval;
* major project changes;
* change orders.

---

## Level 5 — Financial Authorization

Required for financial decisions such as:

* escrow release;
* payment authorization;
* payout-destination modification.

---

## Level 6 — Wallet / Transaction Authorization

Where BMONI financial infrastructure is used, additional requirements may include:

* wallet readiness;
* KYC (Know Your Customer);
* transaction signing;
* BMONI authorization state.

---

## Administrative Privileges

Administrative access should remain distinct from Owner privileges.

An administrator should not automatically possess construction or financial authority simply because they manage the software system.

**Navigation:** [← Previous: 10. Current-to-Future Gap Analysis](#section-10) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 12. Financial / Escrow Architecture Concept →](#section-12)

---

<a id="section-12"></a>

# 12. Financial / Escrow Architecture Concept

The future architecture must distinguish project governance from financial execution.

```text
OWNER
  │
  ▼
STRUCTURA
  │
  ├── Construction Progress
  ├── BOQ
  ├── Quality Evidence
  ├── Certificates
  └── Milestone Eligibility
          │
          ▼
     OWNER DECISION
          │
          ▼
 FINANCIAL AUTHORIZATION
          │
          ▼
 STRUCTURA BACK-END
          │
          ▼
        BMONI
          │
          ▼
 WALLET / FINANCIAL RAIL
          │
          ▼
 TRANSACTION / PAYMENT STATE
          │
          ▼
    STRUCTURA RECORD
          │
          ▼
      AUDIT TRAIL
```

### Important unverified components

The following remain conceptual or require implementation verification:

* actual escrow legal/technical arrangement;
* current wallet model;
* actual project-fund custody model;
* signing mechanism;
* payment recipient model;
* persistent transaction store;
* webhook/event processing;
* real BMONI integration.

**Navigation:** [← Previous: 11. Security and Authorization Model](#section-11) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 13. 7-Track Governance Mapping →](#section-13)

---

<a id="section-13"></a>

# 13. 7-Track Governance Mapping

## Track 1 — Front-end & 3D (Three-Dimensional) Web User Interface

Primary responsibility:

> What does the Owner see and interact with?

Key capabilities:

* onboarding;
* Owner Command Desk;
* BOQ (Bill of Quantities) presentation;
* transaction-state presentation;
* 3D (Three-Dimensional) / BIM (Building Information Modeling) interaction;
* messaging User Interface;
* notifications User Interface;
* report viewing.

Likely areas:

```text
/src/components/
/src/components/3d/
/src/views/
/src/styles/
```

Potential new areas:

```text
/src/features/owner/
/src/features/onboarding/
/src/features/demo/
/src/features/auth/
/src/features/export/
```

---

## Track 2 — Back-end Systems & APIs (Application Programming Interfaces)

Primary responsibility:

> What happens behind the screen?

Key capabilities:

* persistent project data;
* Application Programming Interfaces;
* messaging;
* site logs;
* notification system;
* aggregation;
* BMONI connection support;
* audit persistence.

Likely areas:

```text
/src/api/
/src/services/db/
/src/middleware/
```

Potential new areas:

```text
/src/services/auth/
/src/services/messaging/
/src/services/notifications/
/src/services/reports/
/src/services/audit/
```

---

## Track 3 — AI (Artificial Intelligence) & Computer Vision

Primary responsibility:

> Where can Artificial Intelligence safely assist?

Key capabilities:

* AI-generated SITREP (Situation Report);
* AI Director;
* project summarization;
* evidence interpretation where appropriate;
* computer-vision analysis.

Likely areas:

```text
/src/services/gemini/
/src/prompts/
/src/components/VisualInspectionAI.tsx
```

Potential new areas:

```text
/src/services/ai-director/
/src/domain/ai-reports/
```

---

## Track 4 — FinTech (Financial Technology), Escrow & Financial Compliance

Primary responsibility:

> How is money represented, authorized, tracked and moved safely?

Key capabilities:

* financial authorization;
* escrow workflow;
* BMONI integration;
* financial readiness;
* wallet relationships;
* transaction lifecycle;
* transaction history.

Likely areas:

```text
/src/services/escrow/
/src/types/billing.ts
```

Potential new areas:

```text
/src/services/bmoni/
/src/services/payments/
/src/domain/transactions/
/src/domain/financial-authorization/
/src/domain/financial-readiness/
```

---

## Track 5 — DevOps (Development Operations), Cloud Infrastructure & Security

Primary responsibility:

> How is the platform protected and operated safely?

Key capabilities:

* authentication security;
* secrets;
* sessions;
* deployment;
* environment separation;
* webhook security;
* observability;
* infrastructure.

Likely areas:

```text
/.github/
/scripts/
/src/middleware/
Dockerfile
docker-compose.yml
.env*
```

---

## Track 6 — Construction Domain & Structural Business Logic

Primary responsibility:

> Does the construction logic actually make professional sense?

Key capabilities:

* BOQ (Bill of Quantities);
* project progress;
* materials;
* quality;
* certification;
* milestones;
* change orders;
* payment eligibility;
* EVM (Earned Value Management);
* construction evidence;
* BIM (Building Information Modeling) relationships.

Potential new areas:

```text
/src/domain/boq/
/src/domain/progress/
/src/domain/materials/
/src/domain/quality/
/src/domain/milestones/
/src/domain/change-orders/
/src/domain/evidence/
/src/domain/earned-value/
/src/domain/bim/
```

---

## Track 7 — Product Strategy, QA (Quality Assurance) & Governance

Primary responsibility:

> Are we building the right thing, testing it correctly, and governing it consistently?

Key capabilities:

* Owner User Experience;
* product requirements;
* acceptance rules;
* audit governance;
* documentation;
* reports;
* testing strategy;
* CODEOWNERS governance;
* AI (Artificial Intelligence) authority boundaries.

Likely areas:

```text
/docs/
/tests/
README.md
CONTRIBUTING.md
```

**Navigation:** [← Previous: 12. Financial / Escrow Architecture Concept](#section-12) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 14. Proposed Repository Architecture →](#section-14)

---

<a id="section-14"></a>

# 14. Proposed Repository Architecture

The following labels are important:

**EXISTING** — known from the current repository information.
**PROPOSED** — architectural boundary suggested by this blueprint.
**MODIFIED** — existing area likely to gain broader responsibility.

```text
Structura/
│
├── src/
│   │
│   ├── components/                         [EXISTING]
│   │   └── 3d/                            [EXISTING]
│   │
│   ├── views/                              [EXISTING]
│   ├── styles/                             [EXISTING]
│   ├── api/                                [EXISTING / MODIFIED]
│   ├── middleware/                         [EXISTING / MODIFIED]
│   │
│   ├── services/
│   │   ├── db/                             [EXISTING]
│   │   ├── gemini/                         [EXISTING]
│   │   ├── escrow/                         [EXISTING / MODIFIED]
│   │   │
│   │   ├── auth/                           [PROPOSED]
│   │   ├── bmoni/                          [PROPOSED]
│   │   ├── payments/                       [PROPOSED]
│   │   ├── audit/                          [PROPOSED]
│   │   ├── messaging/                      [PROPOSED]
│   │   ├── notifications/                  [PROPOSED]
│   │   ├── reports/                        [PROPOSED]
│   │   ├── bim/                            [PROPOSED]
│   │   ├── evidence/                       [PROPOSED]
│   │   └── project-health/                 [PROPOSED]
│   │
│   ├── features/
│   │   ├── onboarding/                     [PROPOSED]
│   │   ├── demo/                           [PROPOSED]
│   │   ├── auth/                           [PROPOSED]
│   │   ├── owner/                          [PROPOSED]
│   │   ├── ai-director/                    [PROPOSED]
│   │   └── export/                         [PROPOSED]
│   │
│   ├── domain/
│   │   ├── project/                        [PROPOSED]
│   │   ├── permissions/                    [PROPOSED]
│   │   ├── boq/                            [PROPOSED]
│   │   ├── progress/                       [PROPOSED]
│   │   ├── evidence/                       [PROPOSED]
│   │   ├── materials/                      [PROPOSED]
│   │   ├── quality/                        [PROPOSED]
│   │   ├── milestones/                     [PROPOSED]
│   │   ├── change-orders/                  [PROPOSED]
│   │   ├── financial-authorization/        [PROPOSED]
│   │   ├── financial-readiness/            [PROPOSED]
│   │   ├── transactions/                   [PROPOSED]
│   │   ├── decisions/                      [PROPOSED]
│   │   ├── audit/                          [PROPOSED]
│   │   ├── notifications/                  [PROPOSED]
│   │   ├── earned-value/                   [PROPOSED]
│   │   ├── bim/                            [PROPOSED]
│   │   └── ai-reports/                     [PROPOSED]
│   │
│   ├── data/                               [EXISTING / MODIFIED]
│   │   └── demo/                           [PROPOSED]
│   │
│   ├── constants/                          [EXISTING]
│   │   └── boq.ts                          [EXISTING]
│   │
│   ├── utils/                              [EXISTING]
│   │   └── formulas.ts                     [EXISTING]
│   │
│   └── prompts/                            [EXISTING / MODIFIED]
│
├── tests/                                  [EXISTING / MODIFIED]
│   ├── unit/                               [PROPOSED]
│   ├── integration/                        [PROPOSED]
│   ├── e2e/                                [PROPOSED]
│   ├── domain/                             [PROPOSED]
│   ├── financial/                          [PROPOSED]
│   └── security/                           [PROPOSED]
│
├── docs/                                   [EXISTING / MODIFIED]
├── .github/                                [EXISTING / MODIFIED]
├── scripts/                                [EXISTING / MODIFIED]
│
├── Dockerfile                              [EXISTING]
├── docker-compose.yml                      [EXISTING]
├── package.json                            [EXISTING]
└── package-lock.json                       [EXISTING]
```

The proposed domain directories are not cosmetic.

Their purpose is to prevent business-critical concepts such as:

* milestone;
* BOQ (Bill of Quantities);
* transaction;
* quality;
* audit

from being scattered across unrelated User Interface files and utility functions.

**Navigation:** [← Previous: 13. 7-Track Governance Mapping](#section-13) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 15. Cross-Track Dependency Map →](#section-15)

---

<a id="section-15"></a>

# 15. Cross-Track Dependency Map

One of the most important conclusions is that the seven tracks should not operate as seven isolated silos.

They form a responsibility network.

```text
                       TRACK 7
             PRODUCT / QA / GOVERNANCE
                         │
                         ▼
                OWNER EXPERIENCE
                         │
            ┌────────────┴────────────┐
            ▼                         ▼
         TRACK 1                   TRACK 3
       FRONT-END / 3D              AI
            │                         │
            └────────────┬────────────┘
                         ▼
                      TRACK 2
                      BACK-END
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
       TRACK 6         TRACK 4        TRACK 5
    CONSTRUCTION      FINTECH        SECURITY /
       DOMAIN          ESCROW       INFRASTRUCTURE
```

---

## Example: Escrow Authorization

What appears to the Owner as one button can require:

```text
Front-end
   ↓
Construction-domain eligibility
   ↓
Back-end request
   ↓
Role authorization
   ↓
Financial authorization
   ↓
BMONI transaction
   ↓
Transaction status
   ↓
Audit record
   ↓
Owner User Interface update
```

Track participation:

**Track 1** — User Interface
**Track 2** — Back-end workflow
**Track 4** — Financial Technology
**Track 5** — Security
**Track 6** — Construction eligibility
**Track 7** — Governance / Quality Assurance

This is a mandatory multi-track capability.

**Navigation:** [← Previous: 14. Proposed Repository Architecture](#section-14) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 16. Risk Register →](#section-16)

---

<a id="section-16"></a>

# 16. Risk Register

| Risk                                                                     | Type                                 | Impact          | Current Concern                                        |
| ------------------------------------------------------------------------ | ------------------------------------ | --------------- | ------------------------------------------------------ |
| User Interface claims payment completed when no real settlement occurred | Financial                            | **Critical**    | Current release state is User Interface-confirmed only |
| Weak or absent authentication                                            | Security                             | **Critical**    | Current authentication not verified                    |
| User chooses Owner role without real authorization                       | Security / Governance                | **Critical**    | Role authorization unverified                          |
| BMONI secrets exposed in browser                                         | Security                             | **Critical**    | Must remain server-side                                |
| Construction work becomes financially eligible without verified evidence | Construction / Financial             | **Critical**    | Domain rules not yet established                       |
| Missing audit trail                                                      | Governance / Financial               | **Critical**    | Persistent audit architecture unverified               |
| Duplicate / invalid financial events                                     | Integration                          | **Critical**    | Webhook architecture not yet implemented               |
| Demo data mixes with production data                                     | Security / User Experience           | **High**        | Guest-first model requires isolation                   |
| 3D model disconnected from real project records                          | Technical                            | **High**        | BIM link architecture unknown                          |
| AI-generated information treated as authoritative fact                   | Artificial Intelligence / Governance | **High**        | AI boundaries need enforcement                         |
| Direct Line messages are not persistent                                  | Messaging                            | **High**        | Backend unknown                                        |
| Situation Report generation does not function                            | Product / Demo                       | **High**        | Visible non-functional control                         |
| BOQ calculations cannot be traced                                        | Construction / Financial             | **High**        | Data sources unknown                                   |
| Project progress percentage lacks evidence                               | Construction                         | **High**        | Progress model unverified                              |
| Too many parallel architectural changes before competition               | Schedule                             | **High**        | Scope discipline required                              |
| Attempting mobile Software Development Kit rewrite unnecessarily         | Integration / Schedule               | **High**        | REST API better matches current web stack              |
| Competition demo depends on unfinished production-grade architecture     | Competition                          | **High**        | Sandbox demonstration should be bounded                |
| First-use experience remains overloaded                                  | User Experience                      | **Medium–High** | Current role-first entry is dense                      |
| Complex governance becomes new bottleneck                                | Governance                           | **Medium**      | Multi-track review should be risk-based                |
| Excessive proposed directory restructuring                               | Technical / Schedule                 | **Medium**      | Architecture should evolve incrementally               |

**Navigation:** [← Previous: 15. Cross-Track Dependency Map](#section-15) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 17. Assumptions and Unknowns →](#section-17)

---

<a id="section-17"></a>

# 17. Assumptions and Unknowns

The blueprint intentionally records uncertainty.

## Existing backend

We do not yet know exactly how much of the current User Interface is connected to persistent backend services.

---

## Database

A `/src/services/db/` path has been referenced, but the actual:

* database technology;
* schema;
* persistence model;
* migration strategy

have not been verified.

---

## Authentication architecture

No current identity provider or session strategy has been verified.

---

## Escrow definition

Structura currently uses the word **Escrow**.

It remains necessary to define precisely whether this means:

* a product concept;
* a financial holding mechanism;
* a legally structured escrow arrangement;
* a project-controlled wallet;
* or another implementation.

The word itself must not be treated as proof of an actual escrow arrangement.

---

## BMONI integration status

No working Structura-to-BMONI integration has yet been verified.

---

## BMONI wallet ownership model

It remains unresolved whether the relevant wallet would belong to:

* the Owner;
* the project;
* another authorized party;
* another financial structure.

---

## Transaction-signing architecture

The production mechanism for financial signing remains undecided.

---

## BIM (Building Information Modeling)

The current source, format and stable identifiers of the model are unknown.

This directly affects whether model elements can reliably link to:

* BOQ (Bill of Quantities);
* progress;
* quality;
* milestones;
* financial status.

---

## AI (Artificial Intelligence) implementation

Existing Gemini-related directories indicate AI (Artificial Intelligence) work, but the current AI (Artificial Intelligence) capabilities and data-access patterns remain unverified.

---

## EVM (Earned Value Management)

Metrics appear in the current interface.

Their exact calculation logic and inputs remain unverified.

---

## Site Log persistence

The input modal works.

Successful server persistence remains unverified.

---

## Messaging persistence

User Interface insertion works.

Actual recipient delivery and persistence remain unknown.

---

## Notification infrastructure

Not verified.

---

## Testing coverage

The existence and depth of automated tests have not yet been established.

---

## Production infrastructure

Current hosting, deployment, observability, environment separation and secret-management practices require verification.

**Navigation:** [← Previous: 16. Risk Register](#section-16) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 18. Pre-Backlog Capability Inventory →](#section-18)

---

<a id="section-18"></a>

# 18. Pre-Backlog Capability Inventory

The following represents the capability inventory that can later be decomposed into:

> **Epic → Feature → User Story → Engineering Task → Subtask**

No such decomposition is performed here.

## Product & Onboarding

* Product landing experience
* Visual product tour
* Guest exploration
* Demo Owner environment
* Demo data isolation
* Access My Project
* Returning-user experience

## Identity & Access

* Authentication
* Session management
* Project membership
* Owner role authorization
* elevated authorization
* administrative privileges
* Exit / Switch Role

## Owner Command

* Owner Command Desk
* project-health summary
* decision queue
* project overview

## Project Data

* project entity
* project membership
* project activities
* work packages
* project status

## BOQ (Bill of Quantities)

* BOQ line items
* cost baseline
* approved changes
* current cost
* certified value
* paid value
* outstanding value
* BOQ variance
* BOQ audit relationship

## Progress

* work-progress records
* progress evidence
* progress aggregation
* progress traceability

## 3D (Three-Dimensional) / BIM (Building Information Modeling)

* 3D model viewer
* proposed model
* completed model
* storey isolation
* model layers
* BIM element mapping
* BIM-to-progress relationship
* BIM-to-BOQ relationship
* BIM-to-quality relationship
* BIM-to-milestone relationship

## Site Evidence

* photographs
* evidence metadata
* evidence storage
* evidence relationships
* site log
* materials evidence
* inspection evidence

## Materials

* specifications
* procurement status
* delivery
* inspection
* acceptance
* installation
* BIM relationship

## Quality

* inspections
* QA/QC (Quality Assurance / Quality Control) records
* certificates
* defects
* quality gates
* payment-eligibility relationship

## Milestones

* milestone definition
* milestone lifecycle
* evidence package
* certification
* Owner review
* Owner decision
* financial eligibility

## Change Orders

* change request
* reason
* cost impact
* schedule impact
* BOQ impact
* evidence
* clarification
* decision history

## Reporting

* site logs
* SITREP (Situation Report)
* periodic monitoring
* EVM (Earned Value Management)
* progress reporting
* financial reporting
* structured export

## AI (Artificial Intelligence)

* AI-generated SITREP
* AI Director
* project summarization
* evidence-supported answer generation
* AI authority boundaries
* human review
* AI audit metadata

## Communication

* Direct Line
* persistent messages
* contextual messages
* clarification requests
* notifications
* notification preferences
* transaction notifications

## Financial Technology

* financial authorization
* escrow-state model
* payment eligibility
* payment state
* payout destination
* financial decision history

## BMONI

* BMONI user mapping
* wallet readiness
* KYC (Know Your Customer) state
* financial rail state
* wallet balance
* BMONI Application Programming Interface client
* transaction proposals
* financial signing
* transaction submission
* transaction status
* BMONI event/webhook processing
* sandbox integration
* production integration boundary

## Audit

* decision record
* audit event
* transaction history
* state transition history
* user-action history
* financial references
* evidence references
* exportable audit package

## Security

* secret management
* secure environment variables
* protected routes
* server authorization
* financial authorization
* webhook validation
* environment separation
* observability
* security logging

## Testing

* User Interface tests
* domain tests
* Application Programming Interface tests
* authentication tests
* authorization tests
* financial tests
* BMONI integration tests
* webhook tests
* security tests
* end-to-end tests
* Artificial Intelligence tests

## Governance & Documentation

* 7-Track review rules
* CODEOWNERS
* Product Requirements Document
* architecture documentation
* glossary
* security documentation
* BMONI integration documentation
* domain rules documentation
* test strategy
* audit policy

**Navigation:** [← Previous: 17. Assumptions and Unknowns](#section-17) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 19. Readiness Gate →](#section-19)

---

<a id="section-19"></a>

# 19. Readiness Gate

## A. What is sufficiently understood to enter backlog creation?

The team now has a reasonably coherent understanding of:

* the current Owner screens;
* verified interactions;
* non-functional controls;
* future Owner product concept;
* guest-first onboarding principle;
* major security boundaries;
* relationship between Structura and BMONI;
* 7-Track Governance responsibilities;
* primary capability gaps;
* major system dependencies;
* key risks;
* major proposed architecture boundaries.

This is sufficient to **begin controlled backlog decomposition**, provided unresolved high-risk architectural decisions are clearly marked.

---

## B. What still requires investigation?

Important investigation remains around:

* source code;
* current database;
* current backend;
* current authentication;
* current Gemini integration;
* existing tests;
* deployment architecture;
* persistent messaging;
* BIM (Building Information Modeling) source;
* BOQ (Bill of Quantities) calculation logic;
* EVM (Earned Value Management) calculations;
* current site-log storage;
* audit implementation;
* existing escrow implementation.

---

## C. Which architectural decisions must be made first?

Before high-detail implementation planning, the team should agree on:

1. authentication architecture;
2. project/user/role data model;
3. persistent database model;
4. project-domain boundaries;
5. milestone lifecycle;
6. construction-to-payment eligibility rules;
7. financial-state model;
8. BMONI integration boundary;
9. audit architecture;
10. environment and secret management.

---

## D. Which BMONI questions must be answered?

Before production financial architecture is finalized:

* Which exact BMONI sandbox flow will the competition demonstration use?
* What BMONI user maps to what Structura user?
* What does the wallet represent?
* Who controls the wallet?
* Which financial rail is required?
* What KYC (Know Your Customer) state is necessary?
* How is transaction signing performed?
* How will BMONI transaction state return to Structura?
* Will webhooks be implemented for the demonstration?
* Which elements are sandbox-only?
* Which architecture would change for production?

---

## E. Which security decisions must be approved?

The team must approve:

* authentication provider;
* session strategy;
* role-authorization policy;
* protected route policy;
* financial re-authorization policy;
* secret-management strategy;
* BMONI credential handling;
* webhook security;
* transaction-signing boundary;
* audit immutability expectations;
* demonstration/production environment separation.

---

## F. Which User Experience decisions must be approved?

The team should explicitly approve:

* guest-first onboarding;
* “Experience value before authentication” principle;
* demonstration-data boundaries;
* visual introduction structure;
* when role selection appears;
* authentication triggers;
* financial authorization triggers;
* returning-user flow;
* how incomplete features appear;
* transaction-state language;
* the Owner Command Desk information hierarchy.

**Navigation:** [← Previous: 18. Pre-Backlog Capability Inventory](#section-18) · [↑ Back to Table of Contents](#table-of-contents) · [Next: 20. Final Product Flow Summary →](#section-20)

---

<a id="section-20"></a>

# 20. Final Product Flow Summary

The full future Owner journey can now be summarized in one model.

```text
┌───────────────────────────────┐
│       DISCOVER STRUCTURA      │
└──────────────┬────────────────┘
               ↓
┌───────────────────────────────┐
│       EXPLORE AS GUEST        │
│  Demo Data • Product Tour     │
└──────────────┬────────────────┘
               ↓
┌───────────────────────────────┐
│     SELECT OWNER / CLIENT     │
└──────────────┬────────────────┘
               ↓
      AUTHENTICATE FOR
        REAL PROJECT
               ↓
┌───────────────────────────────┐
│      OWNER COMMAND DESK       │
└──────────────┬────────────────┘
               ↓
              SEE
               │
     ┌─────────┼─────────┐
     ↓         ↓         ↓
   3D/BIM   SITE DATA   MATERIALS
               │
               ▼
          UNDERSTAND
               │
   ┌───────────┼────────────┐
   ↓           ↓            ↓
  BOQ       PROGRESS      SITREPs
   │           │            │
 VARIANCE     EVM         QUALITY
   └───────────┼────────────┘
               ↓
             DECIDE
               │
    ┌──────────┼───────────┐
    ↓          ↓           ↓
MILESTONES  CHANGES    FINANCIAL
                         DECISION
               │
               ▼
     STRONGER AUTHORIZATION
        WHEN REQUIRED
               │
               ▼
            TRANSACT
               │
               ▼
       STRUCTURA BACK-END
               │
               ▼
              BMONI
               │
               ▼
   WALLET / FINANCIAL RAIL
               │
               ▼
      TRANSACTION STATUS
               │
               ▼
          COMMUNICATE
               │
     ┌─────────┼─────────┐
     ↓         ↓         ↓
 DIRECT     REQUEST     NOTIFY
  LINE    CLARIFICATION
               │
               ▼
         RECORD & AUDIT
               │
      ┌────────┼─────────┐
      ↓        ↓         ↓
 DECISIONS  PAYMENTS   REPORTS
      │        │         │
      └────────┼─────────┘
               ↓
      MONITOR PROJECT OUTCOME
               │
               └───────────────┐
                               │
                               ▼
                         OWNER COMMAND
                              DESK
```

The conceptual loop is therefore:

# **SEE → UNDERSTAND → DECIDE → AUTHORIZE → TRANSACT → COMMUNICATE → RECORD → MONITOR**

Structura's Owner / Client experience is no longer understood simply as a collection of dashboards.

It is defined as an **evidence-connected construction project decision environment** in which:

* physical project information;
* construction logic;
* commercial information;
* Owner authority;
* financial infrastructure;
* Artificial Intelligence assistance;
* communication;
* and audit history

work as related parts of one system.

**Navigation:** [← Previous: 19. Readiness Gate](#section-19) · [↑ Back to Table of Contents](#table-of-contents) · [Next: Blueprint Conclusion →](#section-21)

---

<a id="section-21"></a>

# Blueprint Conclusion

The current PoC (Proof of Concept) has already established much of the **visible product language** of Structura.

The next phase should not discard that work.

Instead, engineering should progressively connect those visible concepts to:

```text
Real Identity
      ↓
Real Project Data
      ↓
Construction Rules
      ↓
Evidence
      ↓
Authorized Decisions
      ↓
Secure Financial Actions
      ↓
Actual Transaction State
      ↓
Persistent Audit History
```

This is the boundary between **Structura as a compelling Proof of Concept** and **Structura as an engineered product**.

> **“This blueprint establishes the agreed product and engineering baseline from which the Structura Owner / Client Product Backlog and detailed Work Breakdown Structure (WBS) can now be derived.”**

**Navigation:** [← Previous: 20. Final Product Flow Summary](#section-20) · [↑ Back to Table of Contents](#table-of-contents)

---
