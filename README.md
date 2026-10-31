# Affinity OpenAPI

**This repository does not publish a specification or a package.** The API serves its contract at [api.affinityrx.com/v1/openapi.json](https://api.affinityrx.com/v1/openapi.json). The current `Affinity-Version` is `2026-10-28`. Send that value in the `Affinity-Version` header of every request.

The [API documentation](https://docs.affinityrx.com/) describes authentication, Test and Live mode, and every operation.

## Official SDKs

Fern generates each SDK from this contract. Install the TypeScript SDK from npm; install the others from GitHub at the tag in their README.

| Language | Repository |
| --- | --- |
| TypeScript | [affinity-health/affinity-typescript](https://github.com/affinity-health/affinity-typescript) (`@affinity-health/sdk@next` on npm) |
| Python | [affinity-health/affinity-python](https://github.com/affinity-health/affinity-python) |
| Go | [affinity-health/affinity-go](https://github.com/affinity-health/affinity-go) |
| Java | [affinity-health/affinity-java](https://github.com/affinity-health/affinity-java) |
| C# | [affinity-health/affinity-csharp](https://github.com/affinity-health/affinity-csharp) |

To generate a client in another language, use the live document above.
