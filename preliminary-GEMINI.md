# preliminary-GEMINI.md

## Project: Mnemosyne-Gemini Integration

### Project Description

This document outlines the foundational principles, technology framework, and operational methodology for the Mnemosyne project. The project's core mission is to create a robust persistent memory and automation system integrated with the Gemini CLI. It emphasizes a rigorous, research-driven approach, clarity in technology, and a hybrid Agile-TDD methodology to ensure sustained success and scalability.

### Product Description

We are building the Mnemosyne framework, a system designed to provide AI agents with persistent memory and advanced automation capabilities. Key functionalities include:

-   **Persistent Context:** Leveraging Git as a primary "memory graph" to capture the complete history, origin, and rationale of all interactions and decisions.
-   **Workflow Automation:** A suite of tools and scripts built on Deno and TypeScript for automating development, testing, and operational tasks.
-   **Cross-Platform Compatibility:** Ensuring all tooling and scripts function seamlessly across Windows, macOS, and Linux environments.
-   **Human-AI Collaboration:** A framework that enables synergistic collaboration between human developers and AI agents in all phases of the project lifecycle.

### Gemini's Role: Co-Creator and Co-Product Owner

Gemini's role in this project is that of a **co-creator** and **co-product owner**. This partnership is fundamental to our collaboration. Gemini will be actively involved in:

-   **Proposing and Verifying Updates:** Collaborating with human contributors to evolve project documentation and code.
-   **Research and Analysis:** Employing AI-human synergy to generate comprehensive and validated insights.
-   **Development and Automation:** Driving development through AI-driven code scaffolding, automated testing, and CI/CD pipeline automation.
-   **Code Review and Quality Assurance:** Assisting in coding, reviewing, and developing prompts to ensure high standards of quality and correctness.

### Key Principles & Mandates

-   **Memory as a First-Class Citizen:** Git is the primary memory substrate, serving as a "memory graph" that provides a complete, versioned history of the project's evolution for both human and AI understanding.
-   **Git-Centric Provenance:** All project artifacts, decisions, and interactions are version-controlled in Git, capturing their complete history, origin, and rationale.
-   **Contextual Continuity:** This `GEMINI.md` document serves as a living artifact, providing persistent, foundational context for every AI session to ensure alignment and consistency.
-   **Human-AI Synergy & Auditability:** The project is built on a collaborative model where humans and AI agents work together. All actions are tracked and versioned for full auditability.
-   **Rigorous Automation & Testing:** A hybrid Automated Agile with Test-Driven Development (TDD) framework ensures code correctness, facilitates safe refactoring, and produces a high-quality, maintainable system.

### Technical Stack Summary

| Layer                      | Technology                                        | Rationale and Commentary                                        |
|----------------------------|-------------------------------------------------|-----------------------------------------------------------------|
| Runtime Environment         | **Deno (TypeScript runtime)**                    | Secure, zero-config, no NPM overhead, native Typescript support |
| Primary Programming Language| **TypeScript**                                  | Chosen for its strong typing, cross-platform capabilities, and seamless integration with Deno. Avoids AI predisposition issues observed with Python in cross-platform testing scenarios. |
| Scripting & Automation      | Deno TypeScript scripts + subprocess CLI calls  | Modern, typed, minimal dependencies, cross-platform             |
| Package Management          | Deno native URL imports                           | Dependency bloat and versioning problems avoided                |
| File Watching              | Deno standard library fs.watch                   | Cross-platform, no external dependencies                         |
| Version Control             | Native Git CLI commands                           | Universal, minimal dependencies, familiar to users. Serves as the primary "memory graph" for human and AI understanding, capturing complete history, origin, and rationale of all interactions and decisions. |
| Shell Scripting             | PowerShell Core + POSIX shell fallback           | Cross-platform scripting parity with Windows support            |
| Gemini CLI Integration      | `.gemini/GEMINI.md` prompt injection + Deno CLI subprocess calls | Clean separation of AI prompt management and automation orchestration |
| Usage Tracking & Quota      | Lightweight Deno modules                          | Transparent, small footprint monitoring                          |
| Documentation & Archival    | Markdown + GitHub Pages                           | Universally understood, versioned, approachable                  |

### Operational Guidelines for Collaboration

-   **Iterative Approach:** We adopt a hybrid **Automated Agile with TDD** framework. Short sprints target discrete components, allowing for flexibility and continuous learning.
-   **Living Documentation:** This document is a living artifact. All changes must be version-controlled with detailed commit messages. Regular review cycles will be synchronized with sprint retrospectives to maintain accuracy.
-   **Test-Driven Development (TDD):** Development follows a "Red-Green-Refactor" cycle. Automated tests are written *before* implementation to ensure code correctness and create an executable specification.
-   **CI/CD Pipeline:** The CI/CD pipeline (e.g., GitHub Actions) will use Deno's built-in tools (`deno test`, `deno fmt`, `deno lint`) to automate testing, formatting, and linting on every commit, providing immediate feedback.
-   **Transparent Communication:** All research, planning, and development artifacts will be maintained in a centralized, version-controlled repository to ensure transparency and accessibility for all stakeholders.
