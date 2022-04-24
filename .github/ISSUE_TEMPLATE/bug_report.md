name: Bug report
about: Something isn't working as intended?
title: ""
labels: 'Bug, Meta: Needs triage'
assignees: ''
body:
  - type: markdown
    attributes:
      value: |
        Hello! Thanks for submit the bug report!
        
        Before you proceed, please search in [open issues](https://github.com/7thbeatgames/adofai/issues?q=is%3Aissue+is%3Aopen) to see if your issue or request has already been filed.
        
        Your issue will be closed if maintainers find it is a duplicate. Please upvote previously reported issues, instead of creating a new one. If your issue isn't submitted before, you are good to write a new one.
  
  - type: textarea
    id: summary
    attributes:
      label: Summary
      description: Please briefly describe the bug. Try to summarize the problem in minimum words yet in an effective way.
    validations:
      required: true
  
  - type: input
    id: version
    attributes:
      label: Version
      description: You may find the version info at the bottom of the main menu.
      placeholder: e.g. v0.11.3 (r23)
    validations:
      required: true
  
  - type: input
    id: os
    attributes:
      label: Operating System (OS)
      description: What OS are you using?
      placeholer: e.g. Windows 11 / macOS Monterey (M1/Intel) / iOS / Android / etc.
    validations:
      required: true
  
  - type: input
    id: platform
    attributes:
      label: Platform
      description: What platform are you using?
      placeholer: e.g. Steam / itch.io / App Store / Play Store / etc.
    validations:
      required: true
  
  - type: input
    id: deviceInfo
    attributes:
      label: Device Info
      description: What device are you using?
      placeholer: e.g. iPhone 13 / Samsung Galaxy Note 22 / iPad Air 5th Generation / etc.
    validations:
      required: false
  
  - type: textarea
    id: stepsToReproduce
    attributes:
      label: Steps to Reproduce
      description: Please describe how to reproduce this bug.
      placeholer: |
        1. Step 1
        2. Step 2
        3. Step 3
        4. See error
    validations:
      required: true
  
  - type: textarea
    id: expectedBehavior
    attributes:
      label: Expected Behavior
      description: Please describe what you expected to happen.
    validations:
      required: true
  
  - type: textarea
    id: observedBehavior
    attributes:
      label: Observed Behavior
      description: Please describe what actually happened.
    validations:
      required: true

  - type: input
    id: reproductionRate
    attributes:
      label: Reproduction Rate
      description: How often the bug happens when you try to reproduce it?
      placeholder: e.g. 100%, 33%, rarely, etc.
  
  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: Please copy and paste [Player.log] output. You may open the log path by pressing [Ctrl + Shift + L] on the game screen.
      render: shell

  - type: textarea
    id: notes
    attributes:
      label: Notes
      description: Please write any other comments about this bug.
      render: shell
