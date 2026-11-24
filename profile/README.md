<h2 align="center">SMMly</h2>

<p align="center"><strong>A self-hosted SMM panel for service businesses, agencies and resellers.</strong><br />
A single-installation platform for service catalogues, customer orders, prepaid wallets and administration.</p>

<p align="center">
  <a href="https://smmly.co">Website</a> ·
  <a href="https://github.com/smmly-co">GitHub organization</a> ·
  <a href="https://github.com/smmly-co/docs">Documentation</a>
</p>

---

> **Development status:** SMMly is under active development and security/reliability remediation. It is not currently declared production-ready. The customer API is unavailable and has not been released.

### Product scope

SMMly is being built to bring the operational workflows of a social media marketing business into one self-hosted panel.

- **Service catalogue** — manage social media services, categories, rates and order requirements.
- **Customer orders** — place and track orders, with refill and cancellation workflows only where implemented and supported.
- **Prepaid wallet** — manage customer funding, balances and transaction history.
- **Provider connections** — connect upstream SMM providers through verified integrations.
- **Reseller API** — planned programmatic ordering through customer API credentials; not released.
- **Support** — customer support workflows.
- **Administration** — manage users, services, providers, orders, deposits, refunds, settings and support.

### Platform

The application is a conventional PHP application using PDO and MySQL/MariaDB, designed for self-hosted deployment on standard PHP hosting, including cPanel.

SMMly is intended as a single-installation, single-tenant SMM panel—not a hosted multi-tenant SaaS control plane or a generic marketplace.

### For developers

SMMly intends to preserve established SMM V2 request and response compatibility where verified. The customer API currently returns HTTP 503 and is not available for integration.

See the [API release status](https://github.com/smmly-co/smmpanel-api/blob/main/CONTRACT-STATUS.md) before planning an integration. Do not rely on undocumented or unreleased endpoints.

### Repositories

Browse the **Repositories** tab for projects and resources maintained by SMMly.

### Security

Do not disclose suspected vulnerabilities in public issues. Read our [Security Policy](https://github.com/smmly-co/.github/blob/main/SECURITY.md) before reporting a concern.

<p align="center"><sub>© SMMly</sub></p>
