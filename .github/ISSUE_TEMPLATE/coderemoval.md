---
name: Code Removal Request
about: Request to have your code removed from this repository.
title: Code Removal Request
labels: DevRequest
assignees: ''

---

body:
  - type: markdown
    attributes:
      value: |
        Please fill out the form below to request removal of your code from this repository.

  - type: input
    id: ma-username
    attributes:
      label: MA Forums Username
      description: Your username on the MA Lighting Forums, if applicable.
      placeholder: e.g. LXTater
    validations:
      required: false

  - type: input
    id: defined-author
    attributes:
      label: Defined Author Name
      description: If your code was not linked from MA Forums, provide the author name as it appears on the page.
      placeholder: e.g. John Doe
    validations:
      required: false

  - type: textarea
    id: pages
    attributes:
      label: Pages Containing Your Code
      description: Link to every page that contains code you want removed. One link per line.
      placeholder: |
        https://...
        https://...
    validations:
      required: true

  - type: checkboxes
    id: confirmation
    attributes:
      label: Confirmation
      options:
        - label: I confirm that I am the original author of the code I am requesting to be removed.
          required: true
