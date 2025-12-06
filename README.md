![Apex Authority Banner](https://img.shields.io/badge/Apex%20Technical%20Authority-Deploying%202026%20Standards-blue?style=flat-square)

# DevIdentity-Free-Subdomain-Provisioning-Web-Registry

[![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/DevIdentity-Free-Subdomain-Provisioning-Web-Registry/ci.yml?label=Build&style=flat-square)](https://github.com/chirag127/DevIdentity-Free-Subdomain-Provisioning-Web-Registry/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/DevIdentity-Free-Subdomain-Provisioning-Web-Registry?label=Coverage&style=flat-square)](https://codecov.io/gh/chirag127/DevIdentity-Free-Subdomain-Provisioning-Web-Registry)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square)](./LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/DevIdentity-Free-Subdomain-Provisioning-Web-Registry?style=flat-square)](https://github.com/chirag127/DevIdentity-Free-Subdomain-Provisioning-Web-Registry/stargazers)

---

> **BLUF:** This repository archives the infrastructure and configuration for a community-driven platform that provisions zero-cost, custom subdomains (e.g., `yourname.thedev.id`) for developers. It simplifies web presence by automating CNAME and DNS record management for static hosting providers like GitHub Pages.

**Star ⭐ this Repo if you believe in democratizing developer identity infrastructure!**

---

## 🏛️ Architectural Blueprint

This system, while architecturally defined by the original web registry specifications, is archived in a hardened, reference-only state. The core logic was designed around robust configuration state management, decoupled from any live cloud provider APIs, prioritizing declarative configuration.

text
DevIdentity-Registry/
├── infrastructure/      # DNS/Registry Configuration Schemas (JSON/YAML)
│   ├── schemas/
│   └── terraform_modules/ (Archived: Infrastructure as Code definitions)
├── src/
│   ├── registrar/
│   │   └── cname_processor.js (Core CNAME validation and generation logic)
│   ├── api/             # Front-facing API contracts (if applicable)
│   └── assets/
│       └── frontend_guide.html (Original deployment documentation)
├── .github/
│   └── workflows/
│       └── ci.yml           # Archival CI/CD pipeline definition
├── AGENTS.md            # Apex Authority Directives
├── README.md            # THIS DOCUMENT
└── PROPOSED_README.md


## 📚 Table of Contents

1.  [Architectural Blueprint](#-architectural-blueprint)
2.  [Development Philosophy](#-development-philosophy)
3.  [Initialization & Verification (Archival Mode)](#-initialization--verification-archival-mode)
4.  [🤖 AI Agent Directives (Critical Reference)](#--ai-agent-directives-critical-reference)
5.  [License](#-license)

---

## 💡 Development Philosophy

This project adheres to the **Apex Authority Principles** for maintainability and resilience:

*   **SOLID:** Focused on Single Responsibility Principle, especially separating DNS logic from UI/API layers.
*   **DRY:** Configuration logic (e.g., subdomain naming conventions) is centralized.
*   **YAGNI:** The archived code reflects only the functionality required for the free subdomain service; no future-proofing cruft was introduced.

## 🚀 Initialization & Verification (Archival Mode)

As this project is archived, setup focuses on static analysis and verification of the existing structure, not execution against live DNS.

1.  **Clone Repository:**
    bash
    git clone https://github.com/chirag127/DevIdentity-Free-Subdomain-Provisioning-Web-Registry.git
    cd DevIdentity-Free-Subdomain-Provisioning-Web-Registry
    

2.  **Environment Setup (Assuming Node/HTML Context):**
    bash
    # Assuming standard web stack configuration for validation purposes
    npm install
    

3.  **Verification Scripts (Linting & Validation):**
    | Command | Purpose |
    | :--- | :--- |
    | `npm run lint` | Run static analysis on all JavaScript/HTML files. |
    | `npm run validate:schemas` | Verify all configuration files against schema definitions. |
    | `npm run check:ci` | Verify the `.github/workflows/ci.yml` integrity. |

---

## 🤖 AI Agent Directives (Critical Reference)

<details>
<summary>View Apex Architecture and Verification Commands (AGENTS.md Reference)</summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs. Use `linkup`/`brave` to search for **December 2025 Industry Standards**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** This repository, `DevIdentity-Free-Subdomain-Provisioning-Web-Registry`, is classified as a **Configuration/Web Infrastructure** project, utilizing declarative configuration (HTML/JS for documentation/fronting) layered over potential backend logic.

*   **PRIMARY SCENARIO: INFRASTRUCTURE/CONFIGURATION (Web Standards)**
    *   **Stack:** The front-facing elements rely on **HTML5/CSS3/Vanilla JavaScript (ES2025)** for maximum portability. The core architecture assumes validation against JSON Schemas for registry entries.
    *   **Lint/Format:** **Biome v2** for ultra-fast linting and formatting across HTML/JS/CSS assets. Configuration is managed via `.ometerrc`.
    *   **Testing:** **Playwright** for End-to-End verification of user flows (e.g., successful CNAME lookup documentation). Unit testing leverages standard browser APIs or Jest if complex state management existed.
    *   **Architecture:** **Declarative Configuration Model**. State (the registry) is maintained via immutable, version-controlled files, minimizing runtime complexity.

---

## 4. CORE ARCHITECTURAL PRINCIPLES (Enforced Universally)
1.  **Immutability:** Registry state transitions must be additive or versioned, never destructive in place.
2.  **Idempotency:** Operations must be safe to repeat without causing unintended side effects (crucial for provisioning).
3.  **Auditing:** Every component must log inputs and outputs relevant to external calls (DNS/CNAME resolution checks).

## 5. VERIFICATION COMMANDS
| Context | Command (Use this to verify adherence) |
| :--- | :--- |
| **Static Analysis** | `npx @biomejs/biome check --apply-unsafe ./` |
| **E2E Flow Check** | `npx playwright test --project=chromium` (Verify documentation links work) |
| **Schema Integrity** | `node ./infrastructure/validate_registry.js` (If applicable, verify JSON structure) |

</details>

## 🛡️ License

This work is distributed under the **Creative Commons Attribution-NonCommercial 4.0 International License**.

See the [LICENSE](./LICENSE) file for full details. Commercial use is strictly prohibited without explicit licensing agreement with `chirag127`.
