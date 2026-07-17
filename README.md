# Affinity OpenAPI

The public OpenAPI contract for the Affinity API.

> **Status:** The initial specification and release workflow have not been published yet. This
> repository currently documents the intended contract boundary for review.

This repository will provide the versioned machine-readable contract used to generate Affinity's
official TypeScript, Python, Go, and Java SDKs.

## Planned contents

```text
openapi.json       Public Affinity API contract
CHANGELOG.md       Human-readable API changes by dated version
README.md          Contract usage and compatibility policy
```

## Source of truth

The public document is exported from Affinity's API implementation. Generated SDKs consume the
exported contract; changes are not patched independently into individual language clients.

The contract covers the public platform integration surface, including:

- Authenticated account and access inspection
- Catalog discovery
- Practice management
- Order creation and lifecycle operations
- Webhook endpoint and event operations
- Authentication, idempotency, and dated API-version headers

Internal administration, pharmacy adapters, routing implementation, and clinical authorization
logic are not part of the public contract.

## Compatibility

Clients should send a supported `Affinity-Version` value and pin their SDK version. Before the
first stable release, the contract may change without a long deprecation window. The release policy
and supported-version window will be documented here before production publication.

## Generated SDKs

- [TypeScript](https://github.com/affinity-health/affinity-typescript)
- [Python](https://github.com/affinity-health/affinity-python)
- [Go](https://github.com/affinity-health/affinity-go)
- [Java](https://github.com/affinity-health/affinity-java)

