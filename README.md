# Inferless (inferless)

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
