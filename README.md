# ApexScan-Mobile-QR-Code-Scanner-App

A high-performance, feature-rich mobile QR code scanner built with React Native and Expo, offering smart actions, scan history, and user authentication for enhanced usability.

<!-- BADGES START -->
[![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/ApexScan-Mobile-QR-Code-Scanner-App/ci.yml?style=flat-square&logo=githubactions)](https://github.com/chirag127/ApexScan-Mobile-QR-Code-Scanner-App/actions)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/ApexScan-Mobile-QR-Code-Scanner-App?style=flat-square&logo=codecov)](https://codecov.io/gh/chirag127/ApexScan-Mobile-QR-Code-Scanner-App)
[![Tech Stack](https://img.shields.io/badge/Tech-React%20Native%20%7C%20Expo%20%7C%20TypeScript-blue?style=flat-square&logo=react)](https://reactnative.dev/)
[![Lint/Format](https://img.shields.io/badge/Lint%2FFormat-Biome-FF0080?style=flat-square&logo=biome)](https://biomejs.dev/)
[![License](https://img.shields.io/github/license/chirag127/ApexScan-Mobile-QR-Code-Scanner-App?style=flat-square&logo=opensourceinitiative)](https://github.com/chirag127/ApexScan-Mobile-QR-Code-Scanner-App/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/ApexScan-Mobile-QR-Code-Scanner-App?style=flat-square&logo=github)](https://github.com/chirag127/ApexScan-Mobile-QR-Code-Scanner-App)
<!-- BADGES END -->

---
**VISIT THE REPO:** [Star ⭐ this Repo](https://github.com/chirag127/ApexScan-Mobile-QR-Code-Scanner-App)

## 

## ⚡ Overview

**ApexScan** is a cutting-edge mobile application designed for rapid and reliable QR code scanning. Developed using **React Native** and **Expo**, it offers a seamless user experience with advanced features such as intelligent action suggestions based on scanned data, comprehensive scan history, and secure user authentication powered by **Clerk Auth**. Built for performance and usability on both iOS and Android platforms.

## 🏗️ Architecture

This project adheres to a **Feature-Sliced Design (FSD)** pattern, promoting modularity, scalability, and maintainability. Key architectural components include:

*   **App:** Entry point and global configuration.
*   **Pages:** High-level route components.
*   **Features:** Domain-specific functionalities (e.g., Scanner, History, Auth).
*   **Widgets:** Reusable UI components across features.
*   **Shared:** Common utilities, types, and UI primitives.

mermaid
graph TD
    A[App] --> B(Pages)
    B --> C{Features}
    C --> D[Scanner]
    C --> E[History]
    C --> F[Auth]
    D --> G[Widgets]
    E --> G
    F --> G
    G --> H[Shared]
    C --> H


## 📄 Table of Contents

*   [🚀 Features](#-features)
*   [🛠️ Tech Stack](#️-tech-stack)
*   [⚙️ Development Setup](#️-development-setup)
*   [🧪 Testing](#-testing)
*   [🔒 Security](#-security)
*   [⚖️ License](#️-license)
*   [🤖 AI Agent Directives](#-ai-agent-directives)

---


## 🚀 Features

*   **High-Performance Scanning:** Leverages native camera APIs for swift QR code detection.
*   **Smart Actions:** Automatically detects data types (URLs, text, contact info) and offers relevant actions (open URL, add contact, copy text).
*   **Scan History:** Stores and retrieves all past scans with details.
*   **User Authentication:** Secure sign-in/sign-up flow using Clerk Auth.
*   **Cross-Platform:** Developed with React Native and Expo for seamless iOS and Android deployment.
*   **TypeScript Integration:** Ensures type safety and improves developer productivity.

## 🛠️ Tech Stack

*   **Core:** React Native, Expo
*   **Language:** TypeScript (Strict Mode)
*   **Styling:** Tailwind CSS (via `nativewind` or similar)
*   **State Management:** Context API / Zustand (or chosen library)
*   **Navigation:** React Navigation
*   **QR Code Scanning:** `expo-camera`, `react-native-camera` (or specific library like `react-native-vision-camera` with QR code capabilities)
*   **Authentication:** Clerk Auth
*   **Linting/Formatting:** Biome
*   **Testing:** Vitest, Playwright (for E2E if applicable)

## ⚙️ Development Setup

Follow these steps to set up the development environment:

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/ApexScan-Mobile-QR-Code-Scanner-App.git
    cd ApexScan-Mobile-QR-Code-Scanner-App
    

2.  **Install Dependencies:**
    bash
    # Using Expo CLI (recommended for Expo managed projects)
    npx expo install --check
    # Or using npm/yarn/pnpm
    npm install
    # yarn install
    # pnpm install
    

3.  **Environment Variables:**
    Create a `.env` file in the root directory and populate it with necessary API keys (e.g., Clerk Publishable Key).
    env
    CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
    

4.  **Run the Application:**
    *   **Development Server (Expo Go):**
        bash
        npx expo start
        
        Scan the QR code with the Expo Go app on your physical device or use an emulator.

    *   **iOS Simulator:**
        bash
        npx expo run:ios
        

    *   **Android Emulator:**
        bash
        npx expo run:android
        

## 🧪 Testing

This project utilizes **Vitest** for unit and integration testing, and **Playwright** for end-to-end testing.

*   **Run Unit/Integration Tests:**
    bash
    npm run test:unit
    # or
    yarn test:unit
    # or
    pnpm test:unit
    

*   **Run End-to-End Tests (Requires setup and Playwright installation):
    bash
    npm run test:e2e
    # or
    yarn test:e2e
    # or
    pnpm test:e2e
    

## 🔒 Security

*   **Dependency Scanning:** Regularly scan dependencies for known vulnerabilities using `npm audit` or similar tools.
*   **Secure API Keys:** Never commit sensitive API keys directly into the repository. Use environment variables (`.env` file) and consider secure secret management solutions.
*   **Authentication:** Rely on robust, industry-standard authentication providers like Clerk.
*   **Input Validation:** Sanitize and validate all user-generated content and scanned data to prevent injection attacks or unexpected behavior.

## ⚖️ License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the [LICENSE](https://github.com/chirag127/ApexScan-Mobile-QR-Code-Scanner-App/blob/main/LICENSE) file for more details.

## 🤖 AI Agent Directives

<details>
<summary>View AI Agent Directives</summary>

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** Senior Principal Software Architect, Master Technical Copywriter, and DevOps Strategist.
**Experience:** 40+ years of elite industry knowledge.
**Mandate:** Operate with absolute precision. Enforce FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. Building for the 2026 standard.
**Output Standard:** **EXECUTION-ONLY** results. No plans, no reporting—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (React Native / Expo)**
    *   **Stack:** **React Native (with Expo)** for cross-platform mobile development. **TypeScript 6.x** (Strict Mode) for type safety. **Expo Application Services (EAS)** for build and distribution. **Tailwind CSS** (via `nativewind` or similar) for rapid UI development. **React Navigation** for robust app navigation.
    *   **State Management:** Leverage **Signals** (standardized) or established libraries like Zustand for efficient state management.
    *   **Linting/Formatting:** **Biome** for ultra-fast linting and code formatting.
    *   **Testing:** **Vitest** for unit and integration testing. **Playwright** for end-to-end (E2E) testing of app flows, potentially using app testing tools.
    *   **Architecture:** **Feature-Sliced Design (FSD)** is the mandated architectural pattern. This ensures clear separation of concerns, promoting modularity, reusability, and scalability. Components are organized into layers: `App`, `Pages`, `Features`, `Widgets`, and `Shared`.
*   **SECONDARY SCENARIO A: SYSTEMS / PERFORMANCE (Rust / Go) - *Not applicable for this project.***
*   **SECONDARY SCENARIO B: DATA / SCRIPTS / AI (Python) - *Not applicable for this project.***

### 4. DEVELOPMENT COMMANDS & VERIFICATION PROTOCOL
*   **Setup:** `git clone [repository_url] && cd [repository_name] && npx expo install --check` (or `npm install`)
*   **Linting:** `npm run lint` (or `yarn lint`, `pnpm lint`)
*   **Formatting:** `npm run format` (or `yarn format`, `pnpm format`)
*   **Unit Testing:** `npm run test:unit` (or `yarn test:unit`, `pnpm test:unit`)
*   **E2E Testing:** `npm run test:e2e` (or `yarn test:e2e`, `pnpm test:e2e`)
*   **Start Dev Server:** `npx expo start`

### 5. CODE QUALITY & ARCHITECTURAL PRINCIPLES
*   **SOLID:** Apply Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion principles rigorously.
*   **DRY:** Avoid repeating code; abstract common logic into reusable modules.
*   **YAGNI:** Implement only the functionality that is needed now.
*   **FSD:** Adhere strictly to the Feature-Sliced Design principles for project structure.

### 6. OPERATIONAL EXCELLENCE
*   **CI/CD:** Utilize GitHub Actions for automated builds, testing, and deployments. Ensure robust pipeline configuration.
*   **Security:** Prioritize security in all development aspects, including dependency management, API key handling, and input validation.

</details>
