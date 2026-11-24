# SMMly GitHub repository map

This map records the repositories that currently exist in the SMMly organization and their verified publication status.

## Organization repositories

| Repository | Visibility | Purpose | Current status |
|---|---|---|---|
| [smmpanel-api](https://github.com/smmly-co/smmpanel-api) | Public | API contract, reference documentation, and future client libraries | Initialized; API not released |
| [smmpanel-telegrambot](https://github.com/smmly-co/smmpanel-telegrambot) | Public | Official Telegram integration project | Initialized; bot planned, not released |
| [docs](https://github.com/smmly-co/docs) | Public | Product and developer documentation | Initialized; documentation being built |
| [examples](https://github.com/smmly-co/examples) | Public | Developer integration examples | Initialized; awaiting verified API contract |
| [.github](https://github.com/smmly-co/.github) | Public | Organization profile and community health files | Active |

## Application source

The existing application is [aruntito/smmly](https://github.com/aruntito/smmly), a private PHP application using PDO and MySQL/MariaDB. It remains outside the organization and must stay private unless the owner explicitly approves a transfer or mirror.

The application README identifies it as under security and reliability remediation and says it is not production-ready. The customer API entry point currently returns HTTP 503 before its older implementation. Therefore the public API repository correctly makes no claim that a supported API is currently available.

## Repository responsibilities

### smmpanel-api

The intended source of truth for the versioned external API contract, authentication, supported actions, request and response schemas, error handling, rate limits, and eventually SDKs. Publish supported details only after implementation and verification.

### smmpanel-telegrambot

The home for a future official Telegram integration. It is currently a project placeholder, not a working bot. A release requires a verified API integration, secure token handling, authorization, abuse controls, tests, and setup documentation.

### docs

The central documentation home for product, installation, administration, API, integration, security, backup, upgrade, and troubleshooting guides. Mark unreleased capabilities as planned.

### examples

Small integration examples that follow the verified API contract. Do not add examples for unavailable endpoints or imply unsupported behavior.

## Release and security rules

- Do not publish private application source or internal audit material in public repositories.
- Do not publish API keys, provider credentials, bot tokens, customer data, or production configuration.
- Do not describe planned capabilities as released.
- Do not publish endpoints, SDKs, or bot workflows until implemented, tested, reviewed, and documented.
- Preserve established SMM V2-style conventions only where compatibility is verified against the released implementation.

## Next engineering sequence

1. Complete and verify the private application's security, financial-integrity, and reliability remediation.
2. Define and test the actual external API contract.
3. Publish verified API reference material and SDKs.
4. Build and test the Telegram integration against that supported API.
5. Expand docs and examples from verified product behavior.
6. Pin repositories only when they contain maintained, useful, release-ready material.

## Branding

The official SMMly symbol and wordmark supplied by the owner are the brand source of truth. The former placeholder SVG was removed and must not be reused. The official symbol should be used for the GitHub organization avatar; the wordmark should be used in the organization profile once the original assets are added to the repository.
