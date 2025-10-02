name: Bug Report
description: Create a detailed bug report to help us improve
title: "[DETAILED DESCRIPTIVE SHORT BUG NAME]"
labels: [bug]
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        <p align="center"><em>Thank you for filing a bug report!</em></p>

        > [!IMPORTANT]
        > - Please provide descriptive titles. Bad titles do more harm than good.
        > - Please search existing issues to avoid creating duplicates.
        > - For enhancement requests, please use the Feature Request form instead.
        > - Please describe the issue clearly and provide steps to reproduce it along with screenshots, videos, or logs if possible.

  - type: textarea
    id: bug-description
    attributes:
      label: Describe the bug
      description: Provide a clear, detailed, and concise description of the bug. Avoid vague titles like "it's broken or "doesn't work".
      placeholder: eg. When Cappy poops, the sound loops infinitely until you quit the app.
    validations:
      required: true

  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to reproduce
      description: Provide numbered steps to reproduce this issue so developers can replicate them.
      placeholder: |
        1. Go to '...'
        2. Click on '...'
        3. Feed the capybara
        4. Wait for the pooping event
        5. Event occurs normally
        5. Observe the error: sound loops forever
    validations:
      required: true

  - type: input
    id: expected-behavior
    attributes:
      label: Expected behavior
      description: What did you expect to happen instead?
      placeholder: eg. The sound plays once, then stops.
    validations:
      required: true

  - type: textarea
    id: screenshots
    attributes:
      label: Screenshots or videos
      description: Add screenshots or videos to help explain the problem, if applicable.

  - type: textarea
    id: system-info
    attributes:
      label: System Information
      description: Please provide details about your environment.
      placeholder: |
        - OS: macOS Ventura 13.2.1
        - Device: 2022 M2 MacBook Air 13" 8GB/256GB
        - CappyHappy Version: v0.0.1 (beta)
        - Other relevant details
    validations:
      required: true

  - type: textarea
    id: additional-context
    attributes:
      label: Additional context
      description: Add any other relevant context, logs, or information here. Please censor personal details.
    placeholder: eg. The Capybara continues with its AI events like normal after this, but the sound loops forever. Note that other sounds, like walking or feeding, still play on top of this looping sound.
