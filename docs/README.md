# SMMly Developer Documentation

This directory is the public entry point for SMMly developer-facing documentation.

## Current publication status

The SMMly application is maintained in a separate private repository. Its integration surface is being reviewed before public API documentation or client libraries are released.

We do not publish guessed endpoints, sample credentials, placeholder SDKs, or unverified behavior.

## Compatibility direction

SMMly's product plan preserves compatibility with the established SMM V2 request and response conventions. Any public contract will be documented against a verified implementation and versioned deliberately.

## Planned public resources

- API reference and authentication guidance
- Request and response examples
- Error and retry semantics
- Webhook documentation, if and when supported by the released implementation
- Client libraries and integration examples, after contract verification

## Security

Never place API keys, passwords, customer records, payment details, or other secrets in public issues or example code.

For security concerns, follow the [SMMly Security Policy](../SECURITY.md).

## Release rule

A resource is published as supported only after its behavior has been verified against the release candidate. Until then, treat it as unpublished and do not build production integrations against assumptions.
