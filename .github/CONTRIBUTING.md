# 🤝 Contributing to DevIdentity-Free-Subdomain-Registration-Service

We welcome contributions to enhance the robustness, security, and feature set of the decentralized subdomain registration service. As an Apex Authority project, adherence to high standards is mandatory.

## 1. Guiding Principles (The Apex Mandate)

All contributions must align with the core philosophies of this repository:

*   **Zero-Defect:** Code must be thoroughly tested and linted according to the Apex Toolchain.
*   **Future-Proof:** Prefer modern, scalable standards (e.g., modern DNS handling, robust configuration management).
*   **DRY & SOLID:** Maintain modularity and separation of concerns, especially concerning DNS record management and identity validation.

## 2. Setup & Environment

Before submitting a pull request, please ensure your local environment is configured to meet the project standards. This repository is fundamentally **HTML/DNS Configuration Focused**, but relies on auxiliary scripts for management, which implies standard CI checks.

1.  **Fork the Repository:** Create your own fork of `chirag127/DevIdentity-Free-Subdomain-Registration-Service`.
2.  **Clone:** Clone your fork locally:
    bash
    git clone https://github.com/YOUR_USERNAME/DevIdentity-Free-Subdomain-Registration-Service.git
    cd DevIdentity-Free-Subdomain-Registration-Service
    
3.  **Branching:** Create a new feature branch based off `main` for your changes:
    bash
    git checkout -b feature/your-awesome-enhancement
    

*Note: Since the core is static HTML/DNS records, the primary focus during local setup is validation against the deployment tooling (likely automated via the `ci.yml` workflow).*

## 3. The Contribution Workflow

We utilize the GitHub Flow model, emphasizing small, iterative changes verified by automation.

### A. Bug Fixes
If you find a bug, please report it using the designated **Bug Report Template** in the `.github/ISSUE_TEMPLATE` directory first. If you are fixing a known issue, reference the issue number in your commit message (e.g., `fix: Resolve CNAME validation failure #123`).

### B. Feature Development
New features should be discussed via a new Issue **before** coding begins, unless the change is a minor refactoring or documentation fix.

### C. Pull Request Submission
When you are ready to submit your changes:

1.  **Commit Hygiene:** Ensure your commits are atomic and messages follow Conventional Commits specification.
2.  **Push:** Push your branch to your fork:
    bash
    git push origin feature/your-awesome-enhancement
    
3.  **Open PR:** Open a Pull Request targeting the `main` branch of `chirag127/DevIdentity-Free-Subdomain-Registration-Service`.
4.  **Templates:** Fill out the **Pull Request Template** completely. Ensure you have verified that all required checks (Build Status, Linting) pass before requesting review.

## 4. Code & Design Standards

For any accompanying scripts (e.g., provisioning, validation scripts not present in the core HTML but implied by the service nature), the following standards apply:

*   **Readability:** Code must be self-documenting where possible. Complex logic requires inline JSDoc/Docstrings.
*   **Security Review:** Any changes involving external API calls or user-supplied input (even configuration files) must explicitly address potential injection vectors (DNS/CNAME manipulation).
*   **Testing:** While the core repo is static, any auxiliary scripts *must* achieve minimum 85% test coverage using **Pytest** or equivalent tooling integrated into `ci.yml`.

## 5. Security Disclosures

We take the security of decentralized identity infrastructure extremely seriously. If you discover a security vulnerability, **DO NOT** open a public issue.

1.  Refer to the **Security Policy** located at `.github/SECURITY.md`.
2.  Follow the responsible disclosure process detailed therein.

Thank you for contributing to the DevIdentity project!