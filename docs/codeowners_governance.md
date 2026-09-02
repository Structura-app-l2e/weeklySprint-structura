# Structura Enterprise CODEOWNERS Documentation

## 📊 7-Track Governance Architecture Overview

This document outlines the operational structure and responsibilities defined within the Structura Enterprise `CODEOWNERS` system. Code ownership is divided into **7 isolated architectural tracks** to enforce strict review workflows, safety guardrails, and compliance.

---

## 🏗️ The 7-Track Governance Grid

| Track | Domain Scope | Primary Ownership Group | Guarded System Paths |
| :--- | :--- | :--- | :--- |
| **Track 1** | Front-end & 3D Web UI | `@Structura-app-l2e/frontend-leads` `@Structura-app-l2e/threejs-specialists` | `/src/components/`, `/src/components/3d/`, `/src/views/`, `/src/styles/`, `/public/`, `index.html`, `vite.config.ts` |
| **Track 2** | Back-end Systems & APIs | `@Structura-app-l2e/backend-leads` | `/server.ts`, `/src/api/`, `/src/services/db/`, `/src/middleware/`, `/src/types/server.ts` |
| **Track 3** | AI & Computer Vision | `@Structura-app-l2e/ai-ml-team` | `/src/components/VisualInspectionAI.tsx`, `/src/services/gemini/`, `/src/prompts/`, `/src/utils/imageProcessing.ts` |
| **Track 4** | FinTech, Escrow & Compliance | `@Structura-app-l2e/fintech-leads` | `/src/components/BudgetVarianceEscrow.tsx`, `/src/services/escrow/`, `/src/utils/currencyFormatter.ts`, `/src/types/billing.ts` |
| **Track 5** | DevOps, Cloud Infrastructure & Security | `@Structura-app-l2e/devops-sec` `@Structura-app-l2e/backend-leads` *(Shared)* | `/.github/`, `Dockerfile`, `docker-compose.yml`, `.env*`, `package.json`, `package-lock.json`, `/scripts/` |
| **Track 6** | Domain & Structural Business Logic | `@Structura-app-l2e/domain-experts` | `/src/data/`, `/src/constants/boq.ts`, `/src/utils/formulas.ts` |
| **Track 7** | Product Strategy, QA & Governance | `@Structura-app-l2e/product-lead` `@Structura-app-l2e/qa-team` | `/docs/`, `/tests/`, `README.md`, `LICENSE`, `CONTRIBUTING.md` |

---

## 🛡️ Global Overrides & Fallbacks

* **Global Fallback Rule:** Any file or directory path not explicitly captured by a specific track rule defaults to the core oversight teams.
  * **Fallback Owners:** `@Structura-app-l2e/product-lead` and `@Structura-app-l2e/core-devs`
* **Precedence Rule:** Later rules in the `CODEOWNERS` config file take precedence over earlier ones. For example, while `/src/components/` belongs to the general Front-end Leads, the nested subdirectory `/src/components/3d/` overrides this and routes strictly to the ThreeJS Specialists.
* **Shared Infrastructure:** Core structural dependencies like `package.json` explicitly require co-authoring and approvals from both the **DevOps/Security** team and the **Backend Leads**.

---

## 🗒️ Production Raw Source File

```text
# ==============================================================================
# STRUCTURA ENTERPRISE CODEOWNERS
# Configured for 7-Track Governance Architecture
# ==============================================================================
# Order matters: Later rules override earlier ones for matching paths.
# Each track requires at least one review from its designated team lead/group.

# Global Fallback Owner (Product & Governance Lead)
*                      @Structura-app-l2e/product-lead @Structura-app-l2e/core-devs

# ==============================================================================
# TRACK 1: Front-end & 3D Web UI
# Primary: Web Application Developers, UX Engineers, 3D Graphics Specialists
# ==============================================================================
/src/components/        @Structura-app-l2e/frontend-leads
/src/components/3d/     @Structura-app-l2e/threejs-specialists
/src/views/             @Structura-app-l2e/frontend-leads
/src/styles/            @Structura-app-l2e/frontend-leads
/public/                @Structura-app-l2e/frontend-leads
index.html              @Structura-app-l2e/frontend-leads
vite.config.ts          @Structura-app-l2e/frontend-leads

# ==============================================================================
# TRACK 2: Back-end Systems & APIs
# Primary: Backend Engineers, Database Administrators, System Architects
# ==============================================================================
/server.ts              @Structura-app-l2e/backend-leads
/src/api/               @Structura-app-l2e/backend-leads
/src/services/db/       @Structura-app-l2e/backend-leads
/src/middleware/        @Structura-app-l2e/backend-leads
/src/types/server.ts    @Structura-app-l2e/backend-leads

# ==============================================================================
# TRACK 3: AI & Computer Vision
# Primary: ML Engineers, Prompt Engineers, Computer Vision Specialists
# ==============================================================================
/src/components/VisualInspectionAI.tsx  @Structura-app-l2e/ai-ml-team
/src/services/gemini/                   @Structura-app-l2e/ai-ml-team
/src/prompts/                           @Structura-app-l2e/ai-ml-team
/src/utils/imageProcessing.ts           @Structura-app-l2e/ai-ml-team

# ==============================================================================
# TRACK 4: FinTech, Escrow & Financial Compliance
# Primary: FinTech Engineers, Escrow Systems Lead, Security Auditors
# ==============================================================================
/src/components/BudgetVarianceEscrow.tsx @Structura-app-l2e/fintech-leads
/src/services/escrow/                    @Structura-app-l2e/fintech-leads
/src/utils/currencyFormatter.ts          @Structura-app-l2e/fintech-leads
/src/types/billing.ts                    @Structura-app-l2e/fintech-leads

# ==============================================================================
# TRACK 5: DevOps, Cloud Infrastructure & Security
# Primary: DevOps Engineers, Site Reliability Engineers (SRE), Security Ops
# ==============================================================================
/.github/               @Structura-app-l2e/devops-sec
Dockerfile              @Structura-app-l2e/devops-sec
docker-compose.yml      @Structura-app-l2e/devops-sec
.env*                   @Structura-app-l2e/devops-sec
package.json            @Structura-app-l2e/devops-sec @Structura-app-l2e/backend-leads
package-lock.json       @Structura-app-l2e/devops-sec
/scripts/               @Structura-app-l2e/devops-sec

# ==============================================================================
# TRACK 6: Domain & Structural Business Logic
# Primary: Construction Domain Experts, Structural Engineers, Data Curators
# ==============================================================================
/src/data/              @Structura-app-l2e/domain-experts
/src/constants/boq.ts   @Structura-app-l2e/domain-experts
/src/utils/formulas.ts  @Structura-app-l2e/domain-experts

# ==============================================================================
# TRACK 7: Product Strategy, QA & Governance
# Primary: QA Engineers, Technical Writers, Product Managers
# ==============================================================================
/docs/                  @Structura-app-l2e/product-lead
/tests/                 @Structura-app-l2e/qa-team
README.md               @Structura-app-l2e/product-lead
LICENSE                 @Structura-app-l2e/product-lead
CONTRIBUTING.md         @Structura-app-l2e/product-lead
```
