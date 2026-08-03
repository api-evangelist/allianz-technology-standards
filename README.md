# Allianz Technology Standards (allianz-technology-standards)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

A collection of technology standards and guidelines maintained by Allianz for software development, API design, architecture, and engineering practices. Allianz follows API-first development using OpenAPI specifications, Backend for Frontends (BFF) architecture, and standardized patterns for pagination, sorting, webhooks, and asynchronous processing.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Best Practices, Enterprise Architecture, Guidelines, Software Development, Technology Standards, API Design, OpenAPI

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-04-19

## APIs

### Allianz Trade API Design Standards
Allianz Trade API design guidelines covering REST API conventions, pagination standards (pageSize, page, totalRequired), sorting conventions, asynchronous processing with JobID management, webhook notification patterns, and security requirements for API integrations.

**Human URL:** [https://developers.allianz-trade.com/docs/api-design-guidelines](https://developers.allianz-trade.com/docs/api-design-guidelines)

#### Tags:

 - API Design, Guidelines, REST API, OpenAPI

#### Properties

- [Documentation](https://developers.allianz-trade.com/docs/api-design-guidelines)
- [Portal](https://developers.allianz-trade.com/)

### Allianz Backend Development Standards
Allianz Global Digital Factory backend development standards. Uses Java and Kotlin with Spring Boot for microservices, API-first approach with OpenAPI specifications, Backend for Frontends (BFF) architecture, and comprehensive automated testing practices.

**Human URL:** [https://globaldigitalfactory.allianz.com/blog/finally-talking-about-backend-.html](https://globaldigitalfactory.allianz.com/blog/finally-talking-about-backend-.html)

#### Tags:

 - Backend, Java, Kotlin, Spring Boot, Architecture

#### Properties

- [Documentation](https://globaldigitalfactory.allianz.com/blog/finally-talking-about-backend-.html)

## Common Properties

- [GitHubOrganization](https://github.com/Allianz)
- [Website](https://www.allianz.com/)
- [Blog](https://globaldigitalfactory.allianz.com/)
- [SpectralRules](rules/allianz-technology-standards-spectral-rules.yml)
- [Vocabulary](vocabulary/allianz-technology-standards-vocabulary.yaml)
- [NaftikoCapability](capabilities/standards-compliance-workflow.yaml)

## Features

| Name | Description |
|------|-------------|
| API First Development | Allianz mandates API-first design using OpenAPI specifications before implementation, enabling frontend teams to work with mock servers independently. |
| Pagination Standards | Standardized pagination using pageSize (default 20), page (default 1), and totalRequired parameters with Total-Items and Total-Pages response headers. |
| Asynchronous Processing Pattern | JobID-based pattern for POST/PATCH/DELETE operations returning a job identifier that clients poll until status transitions from pending to processed. |
| Webhook Notification Standards | Standardized webhook patterns with technical and functional notification types, HTTPS requirement, IP whitelisting, and pre-signed URL support. |
| OAuth2 Security Standard | Allianz Trade APIs standardize on OAuth2 client credentials for programmatic API authentication across all API products. |
| Backend for Frontends Architecture | BFF pattern where each backend service serves a single frontend, enabling clean separation and independent product team decisions. |

## Use Cases

| Name | Description |
|------|-------------|
| API Standards Compliance | Verify that Allianz API implementations conform to documented design guidelines for pagination, sorting, webhooks, and authentication. |
| Developer Onboarding | Guide new developers on Allianz technology conventions for Java/Kotlin backend services, Spring Boot frameworks, and OpenAPI documentation. |
| Architecture Review | Use BFF and API-first standards as criteria for architecture reviews and technical decision documentation. |

## Integrations

| Name | Description |
|------|-------------|
| OpenAPI Initiative | Allianz follows the OpenAPI Specification as the standard format for API documentation and developer portal integration. |
| Swagger UI | Swagger UI used to make API documentation live and executable from OpenAPI specifications. |
| Spring Boot | Spring Boot is the standard framework for delivering Allianz backend services with REST, security, caching, and logging. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Allianz Technology Standards Compliance API](openapi/allianz-technology-standards-compliance.yaml)

### JSON Schema

- [tech-standards-standard-schema.json](json-schema/tech-standards-standard-schema.json)
- [tech-standards-standard-rule-schema.json](json-schema/tech-standards-standard-rule-schema.json)
- [tech-standards-standard-list-schema.json](json-schema/tech-standards-standard-list-schema.json)
- [tech-standards-compliance-check-request-schema.json](json-schema/tech-standards-compliance-check-request-schema.json)
- [tech-standards-compliance-violation-schema.json](json-schema/tech-standards-compliance-violation-schema.json)
- [tech-standards-compliance-result-schema.json](json-schema/tech-standards-compliance-result-schema.json)
- [tech-standards-pagination-guideline-schema.json](json-schema/tech-standards-pagination-guideline-schema.json)
- [tech-standards-webhook-guideline-schema.json](json-schema/tech-standards-webhook-guideline-schema.json)

### JSON Structure

- [tech-standards-standard-structure.json](json-structure/tech-standards-standard-structure.json)
- [tech-standards-compliance-result-structure.json](json-structure/tech-standards-compliance-result-structure.json)

### JSON-LD

- [allianz-technology-standards-context.jsonld](json-ld/allianz-technology-standards-context.jsonld)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Allianz Technology Standards Compliance API](capabilities/shared/standards-compliance.yaml) — 5 operations for technology standards compliance

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Allianz Standards Compliance Workflow](capabilities/standards-compliance-workflow.yaml) | Allianz Technology Standards Compliance API | 5 | Enterprise Architect, API Developer, Platform Governance Team |

## Vocabulary

- [Allianz Technology Standards Vocabulary](vocabulary/allianz-technology-standards-vocabulary.yaml) — Unified taxonomy mapping 3 resources, 3 actions, 1 workflow, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Allianz Technology Standards Spectral Rules](rules/allianz-technology-standards-spectral-rules.yml) — 22 rules across 9 categories enforcing Allianz technology standards conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
