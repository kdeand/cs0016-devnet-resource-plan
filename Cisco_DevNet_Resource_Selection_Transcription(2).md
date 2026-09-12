# Cisco DevNet Resource Selection — Transcription

## Use Case 1: Quick Read-Only API Exploration

**Scenario:** A student team needs immediate access to a shared Cisco environment to practice safe read-only API requests. Administrative changes are not required, and the team cannot wait for provisioning.

**Choice: `always-on-sandbox`**

The deciding requirement is **immediate access without waiting for provisioning**. Cisco states that Always-On sandboxes require no reservation or setup time and are shared environments with restricted administrative access. This fits the students’ need for safe, non-admin API practice.

Claims to verify in [Cisco’s official DevNet Sandbox documentation](https://developer.cisco.com/docs/sandbox/):

- **Access:** Available immediately without a reservation.
- **Isolation:** Shared with other users; it is not a private environment.
- **Setup:** No provisioning or setup time is required.
- **Privileges:** Administrative access is restricted, so users generally work with non-admin APIs.

The team should still check the selected sandbox’s catalog entry because its available APIs, permissions, and usage restrictions may vary.

## Use Case 2: Private Configuration Testing

**Scenario:** A development team must test configuration changes with administrative access in a private environment. The team can schedule access, use a VPN, and accept setup time.

**Choice: `reservation-sandbox`**

The deciding requirements are **administrative access** and a **private environment**. Cisco describes reservation sandboxes as private environments that provide administrative access, making them suitable for testing configuration changes.

Claims to verify in [Cisco’s official DevNet Sandbox documentation](https://developer.cisco.com/docs/sandbox/):

- **Access:** Must be scheduled through a reservation.
- **Isolation:** The reserved environment is private rather than shared.
- **Setup:** Provisioning generally takes time before the environment is ready.
- **Connection:** A VPN connection is generally required.
- **Privileges:** Administrative access is provided to sandbox equipment.

The team should verify the exact permissions, setup time, and VPN requirements in the specific sandbox’s official catalog entry.

## Use Case 3: Guided API Concept Practice

**Scenario:** A beginner needs structured, step-by-step learning content before attempting an independent API activity. The immediate goal is guided practice rather than access to administrative devices.

**Choice: `learning-lab`**

The deciding requirement is the beginner’s need for **structured, step-by-step guided practice** before working independently. A Learning Lab is intended for learning concepts through organized exercises, whereas sandboxes primarily provide environments for experimentation and Code Exchange provides sample code.

Claims to verify in Cisco’s [official Learning Labs Center](https://developer.cisco.com/learning/):

- **Access:** Whether signing in or enrolling is required for the selected content.
- **Isolation:** A Learning Lab is learning content, not necessarily a dedicated or private device environment.
- **Setup:** Check whether the chosen lab requires software, accounts, or access to a separate sandbox.
- **Privileges:** Do not assume administrative access; verify whether the activity uses simulated resources, external systems, or limited credentials.

## Use Case 4: Reusable Automation Example

**Scenario:** A developer wants to examine community and Cisco-maintained code repositories for an existing network-automation use case before designing a new solution.

**Choice: `code-exchange`**

The deciding requirement is the developer’s need to **find and examine existing code repositories** before creating a new solution. Cisco Code Exchange provides access to networking-community projects that are curated and maintained by Cisco.

Claims to verify on the [official Cisco Code Exchange page](https://developer.cisco.com/codeexchange/):

- **Access:** Repositories are publicly available through GitHub, but cloning, contributing, or using cloud-development features may have separate account requirements.
- **Isolation:** Code Exchange is a repository-discovery platform, not a private or isolated testing environment.
- **Setup:** Browsing requires no sandbox provisioning, but running a project may require dependencies and configuration described in its README.
- **Privileges:** Code Exchange does not itself provide administrative access to Cisco devices.
- **Usage:** Check each repository’s documentation, license, maintenance status, and required credentials before reuse.

## Official Cisco References

- [Cisco DevNet Sandbox documentation](https://developer.cisco.com/docs/sandbox/)
- [Cisco DevNet Learning Labs Center](https://developer.cisco.com/learning/)
- [Cisco Code Exchange](https://developer.cisco.com/codeexchange/)
