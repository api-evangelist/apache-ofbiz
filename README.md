# Apache OFBiz (apache-ofbiz)

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

Apache OFBiz is an open-source enterprise resource planning (ERP) system providing a suite of integrated business applications for CRM, e-commerce, supply chain management, manufacturing, accounting, order management, inventory, and warehousing. Built on a service-oriented architecture with a service engine, entity engine, and widget framework, OFBiz exposes a REST API plugin allowing any exported service to be invoked via JWT-authenticated HTTP endpoints. Governed by the Apache Software Foundation under the Apache License 2.0. Written in Java with Groovy scripting support.

**URL:** [https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - ERP, CRM, E-Commerce, Business Applications, Apache, Java, Open Source, Supply Chain

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### Apache OFBiz REST API
REST API plugin for Apache OFBiz that exposes any exported OFBiz service as a RESTful endpoint. Clients authenticate via HTTP Basic Auth to obtain a JWT token, then invoke services via GET (with URL-encoded JSON parameters) or POST (with JSON request body). Swagger UI is available at /docs/swagger-ui.html when the plugin is installed.

**Human URL:** [https://github.com/apache/ofbiz-plugins/tree/trunk/rest-api](https://github.com/apache/ofbiz-plugins/tree/trunk/rest-api)

#### Tags:

 - REST, JWT, Service Engine, ERP

#### Properties

- [Documentation](https://github.com/apache/ofbiz-plugins/blob/trunk/rest-api/src/docs/asciidoc/rest-api.adoc)
- [OpenAPI](openapi/apache-ofbiz-rest-api-openapi.yaml)
- [JSONSchema - Token Response Schema](json-schema/apache-ofbiz-token-response-schema.json)
- [JSONSchema - Service Entry Schema](json-schema/apache-ofbiz-service-entry-schema.json)
- [JSONSchema - Service Response Schema](json-schema/apache-ofbiz-service-response-schema.json)

## Common Properties

- [GitHub Repository](https://github.com/apache/ofbiz-framework)
- [GitHub Organization](https://github.com/apache)
- [Documentation](https://ofbiz.apache.org/documentation.html)
- [Getting Started](https://nightlies.apache.org/ofbiz/stable/ofbiz/html5/developer-manual.html)
- [Tutorials](https://cwiki.apache.org/confluence/display/OFBIZ/Home)
- [FAQ](https://ofbiz.apache.org/faqs.html)
- [Release Notes](https://github.com/apache/ofbiz-framework/blob/trunk/CHANGELOG.md)
- [Terms of Service](https://www.apache.org/licenses/LICENSE-2.0)
- [Support](https://ofbiz.apache.org/mailing-lists.html)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/ofbiz)
- [Spectral Rules](rules/apache-ofbiz-spectral-rules.yml)
- [Naftiko Capability](capabilities/apache-ofbiz-erp-operations.yaml)
- [Vocabulary](vocabulary/apache-ofbiz-vocabulary.yaml)
- [JSON-LD Context](json-ld/apache-ofbiz-context.jsonld)

## Features

| Name | Description |
|------|-------------|
| Service-Oriented Architecture | All business logic encapsulated in services accessible via multiple protocols including REST, XML-RPC, and Java. |
| REST API Plugin | Plugin enabling any exported OFBiz service to be invoked via RESTful HTTP endpoints with JWT authentication. |
| JWT Authentication | OAuth2-compatible JWT-based authentication with access tokens and refresh tokens for secure API access. |
| Entity Engine | Flexible data access layer supporting multiple databases with entity-based query API and relationship management. |
| Service Engine | Central business logic executor with transaction management, error handling, and event-driven service chaining. |
| Swagger UI Integration | Built-in Swagger/OpenAPI UI at /docs/swagger-ui.html for API exploration and testing when REST plugin is deployed. |
| Groovy Scripting | Groovy scripting support for service implementations and customizations without Java compilation. |
| Plugin Architecture | Modular plugin system allowing feature extension without modifying core framework code. |
| Multi-Module ERP | Integrated modules for accounting, order management, inventory, manufacturing, CRM, e-commerce, and HR. |
| Widget Framework | XML-based UI component framework for building consistent web interfaces across ERP modules. |

## Use Cases

| Name | Description |
|------|-------------|
| ERP System Integration | Integrate external systems (CRM, WMS, payment processors) with OFBiz via REST API service calls. |
| E-Commerce Backend | Use OFBiz as a headless e-commerce backend with product catalog, pricing, order management, and fulfillment services. |
| Supply Chain Automation | Automate supply chain workflows including purchase orders, inventory updates, and supplier communications via REST services. |
| Accounting Automation | Automate accounting entries, invoicing, AR/AP processing, and financial reporting via OFBiz service API. |
| Manufacturing Operations | Manage manufacturing resource planning, work orders, bill of materials, and production scheduling via OFBiz services. |
| Custom Business Workflows | Build custom business process automations by chaining OFBiz services via the REST API. |

## Integrations

| Name | Description |
|------|-------------|
| Apache Solr | Integration for product and content search indexing across OFBiz data. |
| Groovy | Groovy scripting engine integration for service implementations and data transformations. |
| PostgreSQL | Supported relational database backend via the OFBiz entity engine. |
| MySQL | Supported relational database backend for OFBiz data persistence. |
| Docker | Official Docker support for containerized OFBiz deployments. |
| Swagger UI | OpenAPI documentation and testing interface bundled with the REST API plugin. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Apache OFBiz REST API](openapi/apache-ofbiz-rest-api-openapi.yaml)

### JSON Schema

- [Token Data](json-schema/apache-ofbiz-token-data-schema.json)
- [Token Response](json-schema/apache-ofbiz-token-response-schema.json)
- [Refresh Request](json-schema/apache-ofbiz-refresh-request-schema.json)
- [Service Link](json-schema/apache-ofbiz-service-link-schema.json)
- [Service Entry](json-schema/apache-ofbiz-service-entry-schema.json)
- [Service List Response](json-schema/apache-ofbiz-service-list-response-schema.json)
- [Service Response](json-schema/apache-ofbiz-service-response-schema.json)

### JSON Structure

- [Token Data](json-structure/apache-ofbiz-token-data-structure.json)
- [Token Response](json-structure/apache-ofbiz-token-response-structure.json)
- [Refresh Request](json-structure/apache-ofbiz-refresh-request-structure.json)
- [Service Link](json-structure/apache-ofbiz-service-link-structure.json)
- [Service Entry](json-structure/apache-ofbiz-service-entry-structure.json)
- [Service List Response](json-structure/apache-ofbiz-service-list-response-structure.json)
- [Service Response](json-structure/apache-ofbiz-service-response-structure.json)

### JSON-LD

- [Apache OFBiz Context](json-ld/apache-ofbiz-context.jsonld)

### Examples

- [Token Data](examples/apache-ofbiz-token-data-example.json)
- [Token Response](examples/apache-ofbiz-token-response-example.json)
- [Refresh Request](examples/apache-ofbiz-refresh-request-example.json)
- [Service Entry](examples/apache-ofbiz-service-entry-example.json)
- [Service Response](examples/apache-ofbiz-service-response-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Apache OFBiz REST API](capabilities/shared/apache-ofbiz.yaml) — 5 operations for authentication, service discovery, and invocation

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Apache OFBiz ERP Operations](capabilities/apache-ofbiz-erp-operations.yaml) | Apache OFBiz REST API | 5 | ERP Administrator, Integration Engineer |

## Vocabulary

- [Apache OFBiz Vocabulary](vocabulary/apache-ofbiz-vocabulary.yaml) — Unified taxonomy mapping 2 resources, 5 actions, 1 workflow, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Apache OFBiz Spectral Rules](rules/apache-ofbiz-spectral-rules.yml) — 28 rules across 10 categories enforcing Apache OFBiz REST API conventions

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
