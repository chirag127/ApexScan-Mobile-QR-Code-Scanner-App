---
name: Bug Report
about: Create a report to help us improve
title: "[BUG] "
labels: "bug"
assignees: ""


body:
  - type: markdown
    attributes:
      value: |-
        ## QuickScan QR Code Scanner - Bug Report
        Thank you for helping us improve QuickScan! Please provide as much detail as possible to help us understand and fix the issue.

        **Repository:** [`chirag127/QuickScan-QR-Code-Scanner-Mobile-App`](https://github.com/chirag127/QuickScan-QR-Code-Scanner-Mobile-App)

  - type: input
    id: bug_title
    attributes:
      label: "Concise Summary of the Bug"
      description: "A brief, descriptive title for the bug."
      placeholder: "e.g., App crashes when scanning QR codes with special characters"
    validations:
      required: true

  - type: textarea
    id: bug_description
    attributes:
      label: "Detailed Description"
      description: "Describe the bug in detail. What is happening? What did you expect to happen?"
      placeholder: "Detailed explanation of the bug..."
    validations:
      required: true

  - type: textarea
    id: steps_to_reproduce
    attributes:
      label: "Steps to Reproduce"
      description: "Provide clear, step-by-step instructions on how to reproduce the bug."
      placeholder: "1. Open the app\n2. Navigate to the scanner screen\n3. Scan a QR code with [specific characteristic]..."
    validations:
      required: true

  - type: input
    id: version
    attributes:
      label: "App Version"
      description: "Which version of the QuickScan app are you using? (e.g., 1.0.0)"
      placeholder: "e.g., 1.2.3"
    validations:
      required: true

  - type: input
    id: device_info
    attributes:
      label: "Device Information"
      description: "What device are you using? (e.g., iPhone 15 Pro, Samsung Galaxy S23, Emulator)"
      placeholder: "e.g., iPhone 15 Pro, iOS 17.2"
    validations:
      required: true

  - type: textarea
    id: additional_context
    attributes:
      label: "Additional Context"
      description: "Any other context about the problem. Screenshots, logs, or any other information that can help us resolve the issue faster."
      placeholder: "Paste screenshots, error logs, or any relevant information here..."
    validations:
      required: false

  - type: markdown
    attributes:
      value: |-
        **Tech Stack Alignment:**
        This report pertains to the `chirag127/QuickScan-QR-Code-Scanner-Mobile-App` project, utilizing the following core technologies:
        *   **Framework:** React Native
        *   **Bundler/Environment:** Expo
        *   **Language:** TypeScript
        *   **Styling:** NativeWind
        *   **State Management:** Zustand
        *   **Authentication:** Clerk Auth
        *   **Camera:** Vision Camera
        *   **Platform:** Cross-Platform (iOS/Android)

        Please ensure your bug report aligns with the standards and technologies defined in our AGENTS.md file. For detailed developer directives, refer to the [AGENTS.md](https://github.com/chirag127/QuickScan-QR-Code-Scanner-Mobile-App/blob/main/AGENTS.md) file.