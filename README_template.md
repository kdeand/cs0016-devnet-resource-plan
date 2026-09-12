# IT0123 DevNet Resource Validation Plan

## Student and Project

- Name: Deanna Juliana K. de la Cruz
- Section: TS31
- Repository name: `cs0016-devnet-resource-plan`

## Purpose

Selecting the correct DevNet resource ensures that the environment matches the task’s access, privacy, and learning requirements. Validating the resource beforehand also prevents delays, unsafe configuration attempts, and the use of tools that do not provide the required capabilities.

## Validated Resource Decisions


### UC1 – Quick Read-Only API Exploration
Selected resource: Always-On Sandbox
Most important requirement: The student team needs immediate access to a shared environment for non-administrative API requests without waiting for provisioning.
Official Cisco evidence: Cisco DevNet Sandbox Documentation

Cisco explains that Always-On Sandboxes require no reservation or setup time. These environments are shared, and administrative access is restricted, making this resource appropriate for immediate and safe read-only API exploration.

### UC2 – Private Configuration Testing
Selected resource: Reservation Sandbox
Most important requirement: The team requires a private environment with administrative privileges for testing configuration changes.
Official Cisco evidence: Cisco DevNet Sandbox Documentation

Cisco states that Reservation Sandboxes provide private environments and administrative access. They require a reservation, setup time, and a VPN connection, which the development team is prepared to use.

### UC3 – Guided API Concept Practice
Selected resource: Learning Lab
Most important requirement: The beginner needs structured, step-by-step learning material before performing an independent API activity.
Official Cisco evidence: Cisco DevNet Learning Labs

Cisco presents Learning Labs as interactive tutorials that help users learn by doing. This makes a Learning Lab more appropriate than a sandbox because the immediate goal is guided learning rather than direct access to administrative devices.

### UC4 – Reusable Automation Example
Selected resource: Code Exchange
Most important requirement: The developer needs to examine existing network-automation code and use cases before creating a new solution.
Official Cisco evidence: Cisco Code Exchange

```Cisco Code Exchange provides code projects from the networking community that are curated and maintained by Cisco. These repositories allow developers to study documented automation examples and identify reusable approaches.```

## AI Evaluation

I accepted the AI recommendation to use a Reservation Sandbox for UC2. The scenario requires private access, administrative privileges, and permission to test configuration changes. I independently checked the Cisco DevNet Sandbox documentation and confirmed that Reservation Sandboxes are private, provide administrative access, and generally require a reservation, VPN connection, and setup time.

I modified the evidence links suggested for UC3 and UC4. The original JSON template used the general Sandbox documentation for every use case, but that page did not provide the most direct evidence for Learning Labs or Code Exchange. I replaced those links with the official Cisco DevNet Learning Labs page for UC3 and the official Cisco Code Exchange page for UC4.
## Validation Evidence

- Validator result: PASS
- Command used: 
        ```python3 validate_plan.py```
- Official Cisco pages reviewed:

## Git Evidence

- Initial commit message:
- Validation commit message:
- Output of `git log --oneline`:

## AI-Use Disclosure

State the AI tool used, the type of assistance received, what was independently checked, and what you revised.
