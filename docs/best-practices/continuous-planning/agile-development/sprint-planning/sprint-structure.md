---
title: Structure of a Sprint
summary: A guide to how a sprint should be structured
author: Scott McCarthy
date: 18/08/2022
---

The purpose of this document is to:

- Organize content in the playbook for quick reference and discoverability
- Provide content in a logical structure which reflects the engineering process
- Extensible hierarchy to allow teams to share deep subject-matter expertise

## The first week of a Project

### Before starting the project

Discuss and start writing a team agreement and update these documents with any process decisions made throughout the project.

- [Team Agreement](../team-agreements.md)

  - [Working Agreement](../team-agreements/working-agreements.md)
  - [Definition of Ready](../team-agreements/definition-of-ready.md)
  - [Definition of Done](../team-agreements/definition-of-done.md)
  - [Estimation](estimation.md)

- XXX [Set up the repository/repositories](source-control/README.md#creating-a-new-repository)
  - Decide on repository structure/s
  - XXX Add the following files [README](resources/templates/README.md), [LICENSE](resources/templates/LICENSE), [CONTRIBUTING](resources/templates/CONTRIBUTING.md), .gitignore, etc.
- Build a [product backlog](../backlog-management.md)
  - Set up a project in your chosen project management tool (ex. Azure DevOps or JIRA)
  - [INVEST](<https://en.wikipedia.org/wiki/INVEST_(mnemonic)>) in good user stories and acceptance criteria
  - XXX [Non-Functional Requirements Guidance](design/design-patterns/non-functional-requirements-capture-guide.md)

### Day 1 Activities

- [Plan the first sprint](../sprint-planning.md)

  - Agree on a sprint goal, and how to measure the sprint progress
  - Determine team capacity
  - Assign user stories to the sprint and split user stories into tasks
  - Set up Work in Progress (WIP) limits

- XXX [Decide on test frameworks and discuss test strategies](automated-testing/README.md)
  - Discuss the purpose and goals of tests and how to measure test coverage
  - Agree on how to separate unit tests from integration, load and smoke tests
  - Design the first test cases
- XXX [Decide on branch naming](source-control/naming-branches.md)
- XXX Discuss security needs and verify that secrets are [kept out of source control](continuous-delivery/secrets-management/recipes/azure-devops/secrets-per-branch.md)

### Day 2 Activities

- XXX [Set up Source Control](source-control/README.md)
  - XXX Agree on [best practices for commits](source-control/README.md#commit-best-practices)
- XXX [Set up basic Continuous Integration with linters and automated tests](continuous-integration/README.md)
- Set up meetings for [daily stand-ups](../stand-ups.md) and decide on a Process Lead
  - Discuss purpose, goals, participants and facilitation guidance
  - Discuss timing, and how to run an efficient stand-up
- If the project has sub-teams, set up a [Scrum of Scrums](../scrum-of-scrums.md)

### Day 3

- XXX [Agree on code style](code-reviews/README.md) and on [how to assign Pull Requests](code-reviews/pull-requests.md)
- XXX [Set up Build Validation for Pull Requests (2 reviewers, linters, automated tests)](code-reviews/README.md) and agree on [definition of done](../team-agreements/definition-of-done.md)
- XXX [Agree on a Code Merging strategy](source-control/merge-strategies.md) and update the [CONTRIBUTING](resources/templates/CONTRIBUTING.md) page.
- XXX [Agree on logging and observability frameworks and strategies](observability/README.md)

### Day 4

- Set up [continuous delivery](../../../continuous-delivery.md)
  - Determine what environments are appropriate for this solution
  - For each environment discuss purpose, when deployment should trigger, pre-deployment approvers, sing-off for promotion.
- XXX Decide on a [versioning strategy](source-control/component-versioning.md)
- Agree on how to design a feature and conduct a [design review](../../design-reviews.md)

### Day 5

- Conduct a sprint demo
- Conduct a [retrospective](../../agile-development/retrospectives.md)
  - Determine required participants, how to capture input (tools) and outcome
  - Set a timeline, and discuss facilitation, meeting structure etc.
- [Refine the backlog](../../agile-development/backlog-management.md#backlog-refinement)
  - Determine required participants
  - Update the [definition of ready](../../agile-development/team-agreements/definition-of-ready.md)
  - Update estimates, and the [Estimation](../../agile-development/sprint-planning/estimation.md) document
- XXX Submit [Engineering Feedback](engineering-feedback/README.md) for issues encountered.
