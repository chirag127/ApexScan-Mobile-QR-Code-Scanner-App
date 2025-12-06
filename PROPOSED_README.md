# QuickScan-QR-Code-Scanner-Mobile-App

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/QuickScan-QR-Code-Scanner-Mobile-App/ci.yml?branch=main&style=flat-square)](https://github.com/chirag127/QuickScan-QR-Code-Scanner-Mobile-App/actions/workflows/ci.yml)
[![Codecov](https://img.shields.io/codecov/c/github/chirag127/QuickScan-QR-Code-Scanner-Mobile-App?style=flat-square)](https://codecov.io/gh/chirag127/QuickScan-QR-Code-Scanner-Mobile-App)
[![Tech Stack](https://img.shields.io/badge/Tech%20Stack-React%20Native%20%7C%20Expo%20%7C%20TypeScript-blue?style=flat-square)](https://reactnative.dev/)
[![Lint/Format](https://img.shields.io/badge/Lint/Format-Biome-success?style=flat-square)](https://biomejs.dev/)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-yellow.svg?style=flat-square)](https://creativecommons.org/licenses/by-nc/4.0/)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/QuickScan-QR-Code-Scanner-Mobile-App?style=flat-square)](https://github.com/chirag127/QuickScan-QR-Code-Scanner-Mobile-App)

Star ⭐ this Repo

QuickScan is a high-performance QR code scanner mobile app built with React Native and Expo, offering lightning-fast scanning and secure user authentication. This cross-platform solution provides comprehensive scan history and supports various QR code types for seamless and secure usage.


// Example React Native Component Structure
// Feature-Sliced Design (FSD)

src/
├── app/                 # Entry points, routing, global providers
│   ├── providers.tsx    # Global providers (theme, auth)
│   └── index.tsx        # Root component
├── pages/               # Individual screens or routes
│   ├── home/            # Home screen
│   │   ├── index.tsx    # Home screen component
│   │   └── ui/          # UI components for the home screen
│   ├── scanner/         # QR Scanner Screen
│   │   ├── index.tsx    # Scanner screen component
│   │   ├── lib/          # Scanner logic and utilities
│   │   └── ui/          # UI components for the scanner screen
│   └── history/         # Scan history screen
├── features/            # Independent business logic features
│   ├── qr-scanner/      # QR scanning feature
│   │   ├── api.ts       # API calls related to scanning
│   │   ├── model.ts     # Data models
│   │   └── ui/          # Reusable UI components
│   ├── user-auth/       # User authentication feature
│   │   ├── api.ts       # Authentication API calls
│   │   ├── model.ts       # User data models
│   │   └── ui/          # Authentication UI components
│   └── scan-history/    # Scan history management
├── entities/            # Business entities (User, Product, ScanResult)
│   ├── user.ts          # User entity
│   ├── scanResult.ts    # Scan result entity
│   └── index.ts         # Export all entities
├── shared/              # Reusable modules, UI kit, helpers
│   ├── ui/              # UI Kit (buttons, inputs, etc.)
│   ├── lib/             # Helper functions
│   ├── api/             # Base API client
│   └── config/          # Configuration variables
└── styles/              # Global styles


## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)
- [AI Agent Directives](#ai-agent-directives)

## Features

-   **Lightning-Fast Scanning:** Optimized for quick and accurate QR code detection.
-   **Smart Action Detection:** Automatically identifies and suggests relevant actions (e.g., opening URLs, adding contacts).
-   **Secure User Accounts:** Utilizes Clerk for secure and seamless user authentication.
-   **Comprehensive Scan History:** Maintains a detailed history of all scanned codes.
-   **Cross-Platform Compatibility:** Works on both iOS and Android devices.
-   **Offline Functionality:** Allows scanning even without an internet connection.

## Tech Stack

-   **React Native:** A framework for building native mobile apps using JavaScript and TypeScript.
-   **Expo:** A platform for building universal native apps with JavaScript.
-   **TypeScript:** A superset of JavaScript that adds static typing.
-   **NativeWind:** Uses Tailwind CSS syntax for styling React Native components.
-   **Zustand:** A small, fast, and scalable bearbones state-management solution.
-   **Clerk Auth:** Provides secure user authentication and management.
-   **Vision Camera:** A powerful library for accessing the device's camera.

## Getting Started

1.  Clone the repository:

    bash
    git clone https://github.com/chirag127/QuickScan-QR-Code-Scanner-Mobile-App.git
    cd QuickScan-QR-Code-Scanner-Mobile-App
    

2.  Install dependencies:

    bash
    npm install
    # or
    yarn install
    # or
    pnpm install
    

3.  Configure Environment Variables:

    -   Create a `.env` file in the root directory.
    -   Add your Clerk publishable key:

        
        EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
        

4.  Start the development server:

    bash
    npm start
    # or
    yarn start
    # or
    pnpm start
    

5.  Use the Expo Go app on your iOS or Android device to scan the QR code and run the app.

## Contributing

Contributions are welcome! See the [Contributing Guidelines](https://github.com/chirag127/QuickScan-QR-Code-Scanner-Mobile-App/blob/main/.github/CONTRIBUTING.md) for more information.

## License

This project is licensed under the [CC BY-NC 4.0 License](https://creativecommons.org/licenses/by-nc/4.0/).

## AI Agent Directives

<details>
  <summary>Click to expand</summary>

text
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
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type (`package.json` for React Native) and apply the corresponding **Apex Toolchain**. This repository, `QuickScan-QR-Code-Scanner-Mobile-App`, is a React Native-based mobile application.

*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend)**
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native), WXT (Extensions).
    *   **State:** Signals (Standardized).
    *   **UI Library**: NativeWind (Tailwind CSS in React Native).
    *   **Authentication**: Clerk (Modern Authentication).

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Low Level) - *Not applicable for this project's primary function. Reference only for potential future performance optimizations using native modules.***
    *   **Stack:** Rust (Cargo) or Go (Modules).
    *   **Lint:** Clippy / GolangCI-Lint.
    *   **Architecture:** Hexagonal Architecture (Ports & Adapters).

---

## 4. FILE STRUCTURE & NAMING CONVENTIONS
*   **Feature-Sliced Design (FSD):** The project follows FSD principles for modularity and scalability.
*   **Naming:** Consistent and descriptive naming for components, files, and variables.

---

## 5. DEVELOPMENT STANDARDS
*   **TypeScript Strict Mode:** Enforce strict typing for maximum code safety.
*   **Linting and Formatting:** Use Biome for linting and formatting to maintain code quality.
*   **State Management:** Utilize Zustand for simple and scalable state management.

---

## 6. TESTING & VERIFICATION
*   **Unit Tests:** Use Vitest for unit testing components and logic.
*   **End-to-End Tests:** Use Playwright for end-to-end testing to ensure app functionality.
*   **Command-Line Verification:**
    *   `npm install`: Installs all project dependencies.
    *   `npm run biome`: Runs Biome to check for linting and formatting issues.
    *   `npm run test`: Executes unit tests with Vitest.
    *   `npm run test:e2e`: Executes end-to-end tests with Playwright.


</details>