# Allianz Technology Standards (allianz-technology-standards)
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
