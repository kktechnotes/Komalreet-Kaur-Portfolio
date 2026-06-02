---
title: APIs
parent: Projects
nav_order: 1
---

# Oracle Access Governance REST APIs

## Overview

Oracle Access Governance is an Oracle Cloud Infrastructure (OCI) service that automates and extends **Identity Governance and Administration (IGA)** capabilities, enabling programmatic management of access bundles, self-service request handling, and real-time visibility into permissions and account profiles across integrated systems.

This project covers the **Data Plane REST APIs** — the functional APIs extending Oracle Access Governance Console capabilities.

---

## API Reference Links

| API | Description |
|-----|-------------|
| [Data Plane REST APIs](https://docs.oracle.com/en/cloud/paas/access-governance/pmapi/index.html) | Functional APIs for Access Governance features|
| [Control Plane REST APIs](https://docs.oracle.com/en-us/iaas/api/#/en/access-governance-cp/20220518/) | Service Instance and Administration APIs |

---

## My Involvement

I worked as an individual contributor documenting the end-to-end **Data Plane REST API documentation** for Oracle Access Governance, solely responsible from pulling raw Swagger 2.0 specs from Bitbucket to publishing on `docs.oracle.com`.

### Process

1. **Spec intake & gap analysis:** Pulled auto-generated Swagger 2.0 JSON/YAML from Bitbucket. Audited every endpoint for vague or missing descriptions, undocumented path and query parameters, incomplete enum values, and broken functional flows caused by missing APIs.

2. **Spec authoring:** Edited the following for each endpoint:
   - Resource descriptions
   - Endpoints and methods
   - Parameters
   - Request example
   - Response example

3. **Validation, testing & bug reporting:** Tested all endpoints in **Talend API Tester** (Postman-equivalent). Filed bugs to engineering when API behavior deviated from expected — for example, reporting buggy query parameters or missing APIs that broke functional flows.

4. **Conceptual documentation:** Authored the full developer guide in **DITA/XML**, covering:
   - Quick Start
   - What's New (API release notes)
   - Required Application Roles
   - Authentication and Authorization (OAuth 2.0)
   - Use Cases
   - Response Errors
   - Rate Limiting

5. **Publishing:** Delivered docs through Oracle's CI/CD documentation pipeline for publication on `docs.oracle.com` / OCI Help Center.

---

## Skills

### Technical Writing
- REST API reference documentation (Swagger 2.0 / OpenAPI)
- REST API Getting Started guides
- API release notes (What's New)
- OAuth 2.0 authentication and authorization documentation
- Use case documentation

### Technologies
- **Swagger 2.0** — JSON & YAML spec authoring (path params, query params, examples, enums)
- **DITA / XML** — Structured authoring for examples, use cases, and Getting Started content
- **OAuth 2.0** — Documenting token-based API authentication and authorization flows
- **REST APIs** — HTTP methods, status codes, pagination, rate limiting

### Tools
- **oXygen XML Editor** — Authoring examples, use cases, and Getting Started content
- **Talend API Tester** — Endpoint testing, bug reproduction, and collection authoring
- **Bitbucket** — Source control for spec files and doc content
- **Oracle CI/CD Docs Pipeline** — Publishing to docs.oracle.com
- **Swagger Editor** — Spec validation and preview

---

## Impact

- Sole author of the published Data Plane API reference for a flagship Oracle Cloud service used by enterprise customers globally
- Edited vague auto-generated descriptions with detailed parameter docs and runnable examples for every endpoint
- Identified and reported functional API bugs (broken query parameters, missing APIs causing flow failures), directly improving product quality beyond the documentation scope
- Enabled developer self-service with a complete guide covering Quick Start, Auth, Required Roles, and real-world Use Cases
