# Awesome-Cloud-Metering-Platform

## Top Cloud Metering Platforms Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Usage Metering, Real-Time Aggregation, Usage-Based Billing & Entitlements*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Metering**. These tools help AI, API, and infrastructure companies ingest millions of usage events, aggregate them in real time, enforce entitlements, and generate accurate usage-based invoices.



**Examples** include Metronome, Amberflo, OpenMeter, Orb, Zenskar, Usage.ai, Lago, CloudZero Metering, Sequence, and BillingPlatform (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom metering pipelines, and transparent usage data — ideal for engineering teams that need full control over their usage-based billing infrastructure without revenue-share fees or vendor lock-in.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Metronome](https://metronome.com/)**

  Enterprise-scale usage-based billing platform. Acquired by Stripe in December 2025, completed January 2026. Built for companies with complex contract structures — custom rate cards, annual commitments, credits, overages, and ramps across multiple product lines. Native Stripe integration for payment processing. Free Starter tier available; custom pricing for scaling companies .



- **[Amberflo](https://amberflo.io/)**

  Full-platform usage metering, cost visibility, and customer billing. Connects these into a single system so the same usage data drives both internal cost attribution and customer invoicing. Supports multiple pricing models (per unit, tiered, volume, hybrid) and flexible cost attribution by dimensions .



- **[Orb](https://www.orb.com/)**

  Real-time event ingestion at **250K+ events per second** with custom SQL billable metrics, versioned price migrations, and threshold billing. Strong developer ergonomics and real-time customer-facing usage dashboards. Positions billing as part of the product experience. Custom pricing only (no published rates) .



- **[Zenskar](https://www.zenskar.com/)**

  Usage-based billing platform focused on flexibility and automation. Handles complex pricing models with a visual interface.



- **[Usage.ai](https://www.usage.ai/)**

  AI-powered usage-based billing platform. Automates metering, pricing, and invoicing for consumption-based models.



- **[CloudZero Metering](https://www.cloudzero.com/)**

  Cloud cost intelligence platform with usage metering capabilities. Focuses on internal cost visibility and unit economics rather than customer billing.



- **[Sequence](https://www.sequencehq.com/)**

  Billing and revenue automation platform. Handles subscription billing, invoicing, revenue recognition (ASC 606), and payment collection with embedded finance workflows.



- **[BillingPlatform](https://billingplatform.com/)**

  Enterprise revenue lifecycle management platform with usage-based billing, mediation, and rating capabilities.



## Open-Source GitHub Projects



- **[OpenMeter](https://github.com/openmeterio/openmeter)**

  **The leading open-source metering and billing platform for AI, agentic, and DevTool monetization.** Built in Go with a stack optimized for high-volume event ingestion and real-time aggregation: **PostgreSQL** (billing, subscriptions, entitlements, product catalog), **ClickHouse** (real-time usage aggregation and analytics), and **Kafka** (event streaming pipeline). **Features**: Usage Metering (CloudEvents ingestion, SUM/COUNT/AVG/MIN/MAX aggregations), Usage-Based Billing (tiered, graduated, flat-fee pricing with automated invoice lifecycle), Usage Limits and Entitlements (real-time balance tracking, feature flags, grace periods), Product Catalog (plans, add-ons, features, rate cards, mid-cycle changes with prorating), Prepaid Credits (priority-based burn-down with expiration), Customer Portal (token-based self-service dashboards), Notifications (webhook-based alerts), and LLM Cost Tracking (first-class support for AI token usage). **SDKs**: Go, JavaScript/Node.js, Python. **Apache 2.0** .



- **[Lago](https://github.com/getlago/lago)**

  **The most loved billing solution on GitHub** (6,983 stars, 307 forks). Open-source metering and usage-based billing API chosen by unicorns including **Mistral** (AI, $13.7B valuation), **Swan** (embedded banking), and **Groq** (AI, $6.9B valuation). API-first, no-code interface available. **Five-step billing workflow**: Usage Ingestion (event-based, duplicate prevention), Metrics Aggregation (COUNT, COUNT_UNIQUE, LATEST, MAX, SUM, WEIGHTED SUM), Pricing and Packaging (combine plans and billable metrics for subscription, usage-based, or hybrid models), Invoicing (automated generation with fees, taxes, customer info), and Payments (native integrations or trigger on any PSP). **AGPL-3.0** for self-hosted; **$0 software license**, infrastructure and operations are the customer's responsibility .



- **[Flexprice](https://github.com/flexprice/flexprice)**

  Open-source pricing and billing infrastructure to support **any pricing model** — from usage-based to subscription and everything in between. Designed to eliminate revenue cuts from Stripe and Chargebee. **Architecture**: composable and open — your application, AI agents, or data warehouses send usage data to Flexprice, which handles metering, credits, pricing, billing, and payments in real time. Connects to existing tools for payments, CPQ, CRM, and accounting. **Developer-first design**: API-first, instrument your app by sending usage events via SDKs, Flexprice handles aggregation, metering, and billing logic. **Open-source and self-hostable** for full transparency and control. Supports seat-based subscriptions, usage-based pricing, prepaid credit bundles, and hybrid models. 16 stars (early stage) .



- **[Lotus](https://github.com/uselotus/lotus)**

  **Open-source pricing and packaging infrastructure** (1,738 stars). Python-based. Provides a flexible pricing engine for SaaS applications, supporting usage-based pricing, plan management, experimentation, and integrations with payments and CRM. **MIT License** .



- **[Meterplex](https://github.com/chitrank2050/meterplex)**

  **Open-source B2B usage metering, entitlements, and billing platform.** Built as a **modular monolith** with NestJS 11, TypeScript, PostgreSQL 18 + Prisma 7, Apache Kafka 4.2, and Redis 8. **Key features**: Multi-Tenant Identity & Access (JWT authentication, tenant isolation, Stripe-like API keys with hashed storage), Plans & Entitlements (boolean flags, reset quotas, metered features with snapshotted contracts), Usage Ingestion Pipeline (guaranteed, idempotent delivery via **Transactional Outbox Pattern** and Kafka with concurrency safety), Atomic Aggregations (real-time usage tracking via Postgres raw SQL upserts and Redis caching with TTLs), and Audit-Ready Ledgers (append-only transactional logs with dead-letter auditing). **MIT License** .



- **[Venn](https://github.com/vennbilling/venn)**

  A modern, self-hosted billing platform written in **Clojure**. Early-stage (4 stars) but represents an alternative approach to self-hosted billing infrastructure .



### Additional Strong Open-Source Options



- **Full Metering & Billing**: **OpenMeter** (Go, ClickHouse + Kafka, Apache 2.0, LLM cost tracking) , **Lago** (AGPL-3.0, most adopted, Mistral/Groq backing) , **Flexprice** (composable, any pricing model) .

- **Pricing Infrastructure**: **Lotus** (Python, MIT, pricing and packaging) .

- **B2B Metering**: **Meterplex** (NestJS, Kafka, transactional outbox, entitlements) .

- **API Monitoring + Monetization**: **Moesif** (middleware SDKs for Node.js, Python, Go, Java, Ruby; API monitoring, analytics, and monetization) .



**Frameworks for building custom systems**: Combine **OpenMeter** for real-time metering with ClickHouse + Kafka, **Lago** for the billing workflow (metrics, pricing, invoicing, payments), **Flexprice** for composable pricing across any model, and **Meterplex** for B2B entitlements and audit-ready ledgers. Add **PostgreSQL** for persistence and **Docker** for deployment.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud metering platforms handle sensitive usage and financial data; ensure compliance with relevant data protection and financial regulations.

- **Open-source reality**: The open-source ecosystem for cloud metering is **mature and production-ready**. **Lago** is chosen by unicorns like Mistral and Groq . **OpenMeter** provides a complete real-time metering pipeline with ClickHouse and Kafka, including first-class LLM cost tracking . **Flexprice** and **Meterplex** offer composable and B2B-focused alternatives . Self-hosted deployment requires infrastructure ownership (PostgreSQL, Kafka, ClickHouse, Redis) and engineering time for operations and upgrades — but the software license is free and the data stays under your control.



---



**Made for SaaS founders, AI product engineers, platform teams, and billing infrastructure developers.**

Let's make cloud metering more open, transparent, and scalable.
