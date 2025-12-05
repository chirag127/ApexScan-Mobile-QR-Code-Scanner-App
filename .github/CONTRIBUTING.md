# 🤝 Contributing to ApexScan-Mobile-QR-Code-Scanner-App

As the **Apex Technical Authority**, we welcome contributions that adhere to FAANG-level standards, emphasizing Zero-Defect, High-Velocity, and Future-Proof engineering.

This project utilizes **React Native**, **Expo**, and **TypeScript** (Scenario A stack adapted for Mobile).

## 1. Guiding Principles (The Apex Mandate)

All submissions must align with the core architectural philosophy derived from the **AGENTS.md** directives:

*   **SOLID Compliance:** Ensure all new components and modules adhere strictly to the Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion principles.
*   **DRY & YAGNI:** Avoid code duplication. Only build what is currently required to maintain velocity and simplicity.
*   **Type Safety First:** All new logic in TypeScript must be fully type-checked. Avoid `any` unless absolutely necessary and explicitly justified in the PR description.
*   **Performance Focus:** Given this is a mobile application, prioritize thread safety and minimize re-renders, especially within the camera/scanner module.

## 2. Development Workflow

Follow these steps to ensure your contribution meets integration standards:

1.  **Fork the Repository:** Create your own fork of `chirag127/ApexScan-Mobile-QR-Code-Scanner-App`.
2.  **Clone Locally:** Clone your fork, ensuring you checkout the `main` branch.
3.  **Create a Feature Branch:** Create a new branch for your specific contribution (e.g., `feat/new-scanner-filter` or `fix/auth-token-expiry`).
    bash
git checkout -b my-contribution-branch

4.  **Install Dependencies:** Use the provided setup steps to install the necessary environments.
    bash
# Navigate to project root (assuming root contains package.json)
npm install
# Or using Expo CLI if necessary
npx expo install

5.  **Develop & Test Locally:** Implement your feature or fix. Ensure local testing passes against core functionality.
6.  **Run Static Analysis:** Before committing, ensure the code passes all linter and formatter checks.
    bash
npm run lint
npm run format

7.  **Commit:** Commit changes following the Conventional Commits specification (e.g., `feat: add advanced scanning metadata`).
8.  **Push:** Push your branch to your fork.
    bash
git push origin my-contribution-branch

9.  **Open a Pull Request (PR):** Create a PR targeting the `main` branch of `chirag127/ApexScan-Mobile-QR-Code-Scanner-App`.

## 3. Pull Request Requirements

All Pull Requests **MUST** use the provided template (`.github/PULL_REQUEST_TEMPLATE.md`) and satisfy the following criteria:

*   **Clear Title:** Descriptive title reflecting the change type (feat, fix, chore, refactor).
*   **Detailed Description:** Explain *why* the change is needed and *how* it was implemented.
*   **Verification:** Include steps to verify the change or screenshots/videos if applicable.
*   **Testing Coverage:** If new logic is added, corresponding unit tests (Vitest/Jest compatible) **must** be included and pass CI checks.

## 4. Reporting Issues

If you encounter a bug or wish to propose a significant new feature, please submit an issue using the provided template (`.github/ISSUE_TEMPLATE/bug_report.md`). Be as specific as possible regarding environment (OS, Device model, Expo SDK version).

## 5. Code Style & Formatting

We use **Biome** (as a modern replacement for ESLint/Prettier) for ultra-fast linting and formatting consistency. Your code must adhere to the configuration defined in `biome.json`.

*   **Lint Command:** `npm run lint`
*   **Format Command:** `npm run format`

## 6. Security Disclosure

If you discover a security vulnerability, please follow the established responsible disclosure policy outlined in **.github/SECURITY.md**. Do not report vulnerabilities via public issues or PRs.

--- 

*Thank you for contributing to the Apex Ecosystem.*

**Repository URL for easy reference:** `https://github.com/chirag127/ApexScan-Mobile-QR-Code-Scanner-App`