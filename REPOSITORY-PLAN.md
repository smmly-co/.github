# SMMly GitHub repository plan

This document is the organization-level repository map. It distinguishes existing code from proposed repositories and does not imply that planned repositories or features already exist.

## Existing repositories

| Repository | Visibility | Role | Current status |
|---|---|---|---|
| [.github](https://github.com/smmly-co/.github) | Public | Organization profile, community health, and publication guidance | Exists |
| [aruntito/smmly](https://github.com/aruntito/smmly) | Private | Existing self-hosted PHP SMM panel | Exists outside the organization; under security and reliability remediation |

The private application repository must remain private unless the owner explicitly approves a separate visibility or transfer decision. It is not safe to publish the current application as a public reference implementation.

## Target organization layout

| Proposed repository | Intended visibility | Purpose | Publication gate |
|---|---|---|---|
| smmly-panel | Private | Canonical application source, if/when the owner elects to move or mirror it into the organization | Preserve private visibility; migration/transfer requires explicit owner approval and a reviewed migration plan |
| smmly-api | Public | Versioned API contract, reference documentation, examples, and eventually client libraries | Do not publish as a supported API until the live API contract, authentication, actions, errors, rate limits, and security controls are implemented and tested |
| smmly-telegram-bot | Public only after release review | Official Telegram integration | Requires a real working bot, documented permissions, secure token handling, tests, and supported API integration |
| docs | Public | Product and developer documentation safe for external users | Publish only verified behavior; clearly label unreleased capabilities |
| smmly-examples | Public, optional | Small integration examples and starter projects | Only after the API contract is stable; no credentials or copied customer data |

## Current release blockers

The current private application's README marks the PHP application as under security and reliability remediation and says it is not production-ready. Its customer API entry point currently returns HTTP 503 before the older implementation, explicitly containing an unavailable API. Therefore:

- No public API endpoint should be advertised as operational.
- No SDK should be generated from the disabled or unverified implementation.
- No Telegram bot should be represented as an official working integration until one exists and is tested.
- Do not copy the private application source into a public organization repository.
- Do not publish credentials, production configuration, customer data, or internal audit material.

## Execution sequence

1. Finish and verify application security, financial-integrity, and reliability remediation in the private source repository.
2. Approve whether the canonical application should remain under the personal account or move to the organization as a private repository.
3. Define and test the external API contract against the actual implementation.
4. Publish smmly-api documentation and SDKs only after contract verification.
5. Build and test the Telegram integration against the supported API, then publish it.
6. Publish external documentation and examples, then pin only repositories that are real, maintained, and ready for public use.

## Organization presentation

The official SMMly symbol and wordmark supplied by the owner are the brand source of truth. The former placeholder SVG is not an approved logo and must not be used as brand artwork. Upload the official symbol as the GitHub organization avatar and use the official wordmark in the organization profile after the image assets are committed.

## Tooling limitation

The connected GitHub integration currently supports repository inspection and file/branch operations, but does not expose repository creation, organization profile settings, avatar upload, or repository pinning. Those owner-level operations must be completed through GitHub's organization interface or another authorized workflow. This limitation must not be represented as completed work.
