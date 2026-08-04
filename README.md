# Inferless (inferless)

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

Inferless is a serverless GPU inference platform for machine learning models. Teams import a model from Hugging Face, a Git repo, or a container and Inferless auto-generates a scalable REST inference endpoint billed per second of GPU compute. A workspace-scoped management API and CLI cover model import, deployment, settings, logs, secrets, and volumes.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/apis.yml)

## Tags

- AI
- ML Inference
- Serverless GPU
- Model Deployment
- Inference

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Inferless Inference Endpoints API

Each deployed model exposes an auto-generated REST inference endpoint on a per-deployment host (m-<id>.<region>.model-v1.inferless.com) accepting a KServe v2 style inputs[] payload with name, shape, datatype, and data, secured with a workspace API key as a Bearer token and billed per second of GPU compute.

- **Human URL:** [https://docs.inferless.com/api-reference/model-endpoint/model-endpoint](https://docs.inferless.com/api-reference/model-endpoint/model-endpoint)
- **Base URL:** `https://api.inferless.com`

#### Tags

- Inference
- Serverless GPU
- Predictions

#### Properties

- [Documentation](https://docs.inferless.com/api-reference/model-endpoint/model-endpoint)
- [API Reference](https://docs.inferless.com/api-reference/model-endpoint/test-your-model-endpoint)
- [OpenAPI](openapi/inferless-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/inferless.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/inferless.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Inferless Model Management API

Workspace-scoped REST management API under https://api.inferless.com/rest for updating model autoscaling and machine settings (min/max replicas, machine type, concurrency, inference timeout) and retrieving model runtime logs, secured with a workspace API token.

- **Human URL:** [https://docs.inferless.com/api-reference/model-management-apis/model-settings-update](https://docs.inferless.com/api-reference/model-management-apis/model-settings-update)
- **Base URL:** `https://api.inferless.com`

#### Tags

- Model Management
- Deployments
- Settings
- Logs

#### Properties

- [Documentation](https://docs.inferless.com/api-reference/model-management-apis/model-settings-update)
- [API Reference](https://docs.inferless.com/api-reference/model-management-apis/model-logs-get)
- [OpenAPI](openapi/inferless-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/inferless.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/inferless.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Inferless Workspaces and Deployments

Workspace, model import, and deployment workflow exposed through the Inferless CLI (inferless init, deploy, run, remote-run, model, workspace, runtime, secrets, volume) and backing platform APIs for promoting a model from import to a live serverless inference endpoint.

- **Human URL:** [https://docs.inferless.com/model-import/cli-import](https://docs.inferless.com/model-import/cli-import)
- **Base URL:** `https://api.inferless.com`

#### Tags

- Workspaces
- Imports
- Deployments
- CLI

#### Properties

- [Documentation](https://docs.inferless.com/model-import/cli-import)
- [API Reference](https://docs.inferless.com/references/cli/inferless-deploy)
- [OpenAPI](openapi/inferless-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/inferless.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/inferless.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/inferless)
- [LinkedIn](https://www.linkedin.com/company/inferless)
- [Website](https://www.inferless.com)
- [Documentation](https://docs.inferless.com)
- [Plans](plans/inferless-plans-pricing.yml)
- [Rate Limits](rate-limits/inferless-rate-limits.yml)
- [Fin Ops](finops/inferless-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
