---
title: Integration Guide
parent: Projects
nav_order: 2
---

# Generic REST Integration — Oracle Access Governance

## Overview

This project documents one of the integrations available in Oracle Access Governance. It is an identity and access administration platform for governing and managing access across enterprise applications.

Organizations use fragmented third-party applications for managing and provisioning enterprise accounts. **Generic REST (Standard UI-driven)** is the integration method to bring these fragmented apps under one integration to govern accesses and manage applications. Administrators configure the entire integration through the Oracle Access Governance Console by configuring various REST APIs inside a single connector.

---

## Documentation Links

| Article | Type | Description |
|---------|------|-------------|
| [Integrate with Generic REST (Standard UI-driven)](https://docs.oracle.com/en-us/iaas/Content/access-governance/integrate-with-generic-rest-standard.htm) | Conceptual | Architecture, functional flow, use cases |
| [Configure Integration with Generic REST (Standard UI-driven)](https://docs.oracle.com/en-us/iaas/Content/access-governance/configure-generic-rest-standard.htm) | Configuration | Prerequisites, step-by-step setup, post-configuration |
| [Generic REST Reference (Standard UI-driven)](https://docs.oracle.com/en-us/iaas/Content/access-governance/generic-rest-reference-standard.htm) | Reference | API request/response examples |

---

## My Involvement

complete documentation set for this feature, following the full Documentation Development Lifecycle (DDLC) from requirements analysis through publication.

### Process

1. **Ticket triage & scoping:** Triaged feature documentation ticket, reviewed engineering specs and JIRA context to scope the documentation needed and identify gaps.

2. **Understanding Context:** Retrieved Integration Architecture and Design metholodgy from Confluence (internal engineering wikis, design docs, feature specs) to establish a foundation before engaging with the team and drafted boilerplate content.

3. **SME engagement:** Attended demos with the feature's Point of Contact (POC) engineers to understand the end-to-end integration flow, clarify supported use cases, and gather real-world configuration examples.

4. **Authoring — three-article structure:** Documented the feature as three distinct article types in **DITA/XML** using **oXygen XML Editor**:
   - **Conceptual:** Includes integration overview, architecture, functional flow of the configuration, and supported use cases — written for security administrators and IAM administrators
   - **Configuration:** Includes prerequisites, step-by-step configuration of each component (credentials, permissions, lookups, account schema, authentication APIs, lifecycle APIs), and post-configuration validation steps
   - **Reference:** Includes REST API request/response examples for real operations — Create Account, Group Search, Country Lookup, Add Group Membership, Delete Account

5. **Validation & testing:** Verified configuration steps and API examples for accuracy against the actual product UI and behavior.

6. **Review & approval:** Submitted content for review via **pull requests (PRs)** in **OCI DevOps**. Addressed feedback from engineers, product managers, and peer writers through the PR review cycle.

7. **Publishing:** Merged and published through Oracle's **docs-as-code CI/CD pipeline** to `docs.oracle.com` / OCI Help Center.

---

## Skills

### Technologies
- **DITA / XML** — Structured authoring for modular, topic-based documentation
- **REST APIs** — Reading and documenting API request/response structures, authentication flows, HTTP methods, JSON payloads
- **OAuth 2.0 / Bearer Token authentication** — Documenting token-based and credential-based auth patterns
- **Git / docs-as-code** — PR-based review workflow and CI/CD publishing pipeline

### Tools
- **oXygen XML Editor** — Primary authoring environment for DITA content
- **OCI DevOps** — Source control, PR-based review workflow, and CI/CD publishing pipeline
- **Confluence** — Sourcing engineering background content and internal specs

---

## Impact

- Enabled faster customer onboarding and adoption of Oracle Access Governance by delivering end-to-end integration documentation that combined architecture guidance, configuration workflows, and practical implementation examples
- Documented a complex, multi-step REST integration process into a structured Conceptual, Task and Reference documentation framework for security and IAM administrators with varying levels of technical expertise.
- Delivered a complete documentation set through Oracle's docs-as-code pipeline, ensuring feature readiness and public availability alongside product release timelines.
