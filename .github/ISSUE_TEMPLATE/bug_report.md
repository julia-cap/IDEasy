name: Bug report
description: Create a report to help us improve!
labels:

- bug
  body:
- type: markdown
  attributes:
  value: |
- type: textarea
  id: expected
  attributes:
  label: Actual behavior
  description: Please give a clear and concise description of the bug/actual behavior.
  validations:
  required: true
- type: textarea
  id: reproduce
  attributes:
  label: Reproduce
  description: Steps to reproduce the bug
  placeholder: |
  1. ide create ...
  2. ide upgrade ...
     validations:
     required: true
- type: textarea
  id: expected
  attributes:
  label: Expected behavior
  description: What is the expected behavior?
  placeholder: |
  E.g. `ide upgrade` should update your IDEasy to latest available version
- type: textarea
  id: version
  attributes:
  label: ideasy version
  description: Output of `ide -v`
  render: bash
  placeholder: |
  2025.04.001-04_08_02-SNAPSHOT
  validations:
  required: true
  - type: textarea
    id: info
    attributes:
    label: docker info
    description: Output of `ide status`
    render: bash
    placeholder: |

        IDE_ROOT is set to C:\projects
        IDE_HOME is set to C:\projects\IDEasy
        You are online.
        Your settings are up-to-date.
        Your version of IDEasy is 2025.04.002-04_17_02-SNAPSHOT but version 2025.04.002-20250417.024201-5 is available. Please run the following command to upgrade
        to
        the latest version:
        ide upgrade
        Your operating system is windows(10.0)@x64 [Windows 11@amd64]

  validations:
  required: true
- type: input
  id: related
  attributes:
  label: Related/Dependent Issues
  description: |
  Please state any related or dependent issue...
  validations:
  required: false
- type: input
  id: os
  attributes:
  label: Web browser
  description: |
  Please state your used web browser, if applicable.
  placeholder: |
  Chrome/Firefox/Safari
  validations:
  required: false
- type: textarea
  id: comments
  attributes:
  label: Comments/Hints
  description: Any comments, hints or additional info you want to provide.
  validations:
  required: false
