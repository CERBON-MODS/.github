name: BUG/ISSUE Template
description: Use this template if you’ve discovered a bug or are experiencing an issue.
title: "[BUG/ISSUE] [<Minecraft/Loader Version>] -"
labels: ["bug"]
assignees:
- CerbonXD
  body:
- type: markdown
  attributes:
  value: |
  ## Before submitting the issue
  Please make sure you have checked the following before submitting your issue.

- type: checkboxes
  id: pre_checks
  attributes:
  label: Pre-flight Checks
  options:
  - label: **I have checked that the bug is not a duplicate or, if it is, it needs to be reopened**
  required: true
  - label: **I have checked that I am running the latest version of Bosses of Mass Destruction Mod**
  required: true
  - label: **I have checked the [FAQ](https://github.com/CERBON-MODS/.github/blob/master/FAQ.md) section for solutions**
  required: true
  - label: **I have read the [contributing guidelines](https://github.com/CERBON-MODS/.github/blob/master/CONTRIBUTING.md#issues) and I agree with the [Code of Conduct](https://github.com/CERBON-MODS/.github/blob/master/CODE_OF_CONDUCT.md)**
  required: true

- type: input
  id: versions
  attributes:
  label: Loader, loader version and minecraft version
  description: "Please provide the loader, loader version and the Minecraft version on which you are running the mod."
  placeholder: "For example, Forge 47.2.0, Minecraft 1.20.1"
  validations:
  required: true

- type: textarea
  id: description
  attributes:
  label: Describe the bug
  description: A clear and concise description of what the bug is.
  validations:
  required: true

- type: textarea
  id: reproduce
  attributes:
  label: To reproduce
  description: Steps to reproduce the behavior.
  value: |
  1. Go to '...'
  2. Click on '....'
  3. Scroll down to '....'
  4. See error
  validations:
  required: true

- type: textarea
  id: expected
  attributes:
  label: Expected behavior
  description: A clear and concise description of what you expected to happen.
  validations:
  required: true

- type: textarea
  id: screenshots
  attributes:
  label: Screenshots
  description: If applicable, add screenshots to help explain your problem. You can drag and drop images directly into this box.
  validations:
  required: false

- type: textarea
  id: logs
  attributes:
  label: Latest log
  description: Please paste the latest log here. You can find it by opening the folder where Minecraft is installed, searching for the "logs" folder, opening the "latest.log" file, and copying its content.
  render: log
  validations:
  required: true

- type: textarea
  id: context
  attributes:
  label: Additional context
  description: Add any other context about the problem here.
  validations:
  required: false