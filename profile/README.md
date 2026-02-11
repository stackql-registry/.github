<!-- web assets -->
[logo]: https://stackql.io/img/stackql-logo-bold.png "stackql logo"
[homepage]: https://stackql.io/
[docs]: https://stackql.io/docs
[blog]: https://stackql.io/blog

<!-- repos and links -->
[core]: https://github.com/stackql/stackql
[deploy]: https://github.com/stackql/stackql-deploy
[registry]: https://github.com/stackql/stackql-provider-registry
[license]: https://github.com/stackql/stackql/blob/main/LICENSE
[contributing]: https://github.com/stackql/stackql/blob/main/CONTRIBUTING.md
[discussions]: https://github.com/orgs/stackql/discussions
[openapisaurus]: https://github.com/stackql/openapisaurus
[google2openapi]: https://github.com/stackql/google-discovery-to-openapi
[aws2openapi]: https://github.com/stackql/aws-cfn-schema-to-openapi
[azure2openapi]: https://github.com/stackql/stackql-azure-openapi
[anysdk]: https://github.com/stackql/any-sdk

<!-- orgs -->
[stackql-org]: https://github.com/stackql
[stackql-labs-org]: https://github.com/stackql-labs

<!-- badges -->
[latestreleasebadge]: https://img.shields.io/github/v/release/stackql/stackql?sort=semver "Latest Release"
[orgstars]: https://img.shields.io/github/stars/stackql?style=flat&label=org%20stars "GitHub Org Stars"
[licensebadge]: https://img.shields.io/github/license/stackql/stackql "License"

[openapi]: https://img.shields.io/badge/openapi-%236C757D.svg?plastic&logo=openapiinitiative&logoColor=white
[typescript]: https://img.shields.io/badge/typescript-%23007ACC.svg?plastic&logo=typescript&logoColor=white
[javascript]: https://img.shields.io/badge/javascript-%23323330.svg?plastic&logo=javascript&logoColor=white
[deno]: https://img.shields.io/badge/deno-000000?v&logo=deno&logoColor=white

<!-- social -->
[twitter]: https://twitter.com/stackql
[discord]: https://discord.com/invite/xVXZ9d5NxN

<!-- language: lang-none -->
<div align="center">

[![logo]][homepage]  
![latestreleasebadge]
![orgstars]
![licensebadge]

</div>

<div align="center">

### 🗂️ Provider development projects, OpenAPI source specs, utilities and documentation sites for StackQL providers.

[__⭐ Star the core project »__][core] · [__📖 Docs »__][docs] · [__💬 Discussions »__][discussions]

</div>

---

## About This Organisation

**`stackql-registry`** contains the provider development ecosystem for [StackQL](https://stackql.io). This includes OpenAPI source specifications, provider-specific build and generation tooling, and documentation sites for individual StackQL providers.

> 🔗 **Looking for the main project?** The StackQL core project, the published provider registry (deployed using Deno Deploy), client libraries, and GitHub Actions all live in the [__`stackql`__][stackql-org] organisation.

## What You'll Find Here

This org houses the upstream source materials and tooling used to build and publish StackQL providers, including OpenAPI source specifications for individual cloud and SaaS providers, provider documentation sites (e.g. provider-specific docs deployed via GitHub Pages), build pipelines and generation scripts for provider definitions, and test suites for provider interface validation.

The published, consumable provider registry that StackQL uses at runtime lives at [__`stackql-provider-registry`__][registry] in the core org.

## How StackQL Providers Work

StackQL providers are defined using OpenAPI specifications with StackQL-specific extensions. The provider development pipeline typically follows this flow:

1. **Source specs** (in this org) — raw or transformed OpenAPI definitions from cloud provider documentation
2. **Generation tooling** (in [__`stackql`__][stackql-org]) — tools like [`@stackql/provider-utils`](https://www.npmjs.com/package/@stackql/provider-utils)
3. **Published registry** — the [__`stackql-provider-registry`__][registry] consumed by [`stackql`][core] via [`any-sdk`][anysdk]

## Our Organisations

| Organisation | Purpose |
|---|---|
| [__`stackql`__][stackql-org] | **Core projects** — engine, deploy, registry, client libraries, GitHub Actions. **Start here.** |
| [__`stackql-labs`__][stackql-labs-org] | **Experimental** — proof-of-concepts, emerging integrations |
| **`stackql-registry`** | **Provider development** — OpenAPI source specs, build tooling, documentation sites *(📍 you are here)* |

## Contributing Providers

Interested in adding a new provider or improving an existing one? StackQL's config-file-based provider plugin approach lowers the entry barrier compared to traditional code-intensive plugin frameworks — if a service has an OpenAPI spec, it can become a StackQL provider.

- [**Contributing Guidelines**][contributing]
- [**Discussions & Support**][discussions]

📜 StackQL is released under the [MIT License][license].

---

<div align="center">

🌐 [Website][homepage] · [X][twitter] · [Discord][discord]

</div>
