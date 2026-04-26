# Grierson

> Women's health & wellbeing platform — appointment scheduling, medical records, cycle tracking, and mental wellbeing in one place.

Named after **Cecilia Grierson** (1856–1934), Argentina's first female physician and pioneer of women's healthcare.

## Vision

Women manage their health across fragmented tools. Grierson brings it together: a unified longitudinal health record that understands the whole person — not just isolated symptoms.

## Stack

- **Backend**: PHP 8.4 / Symfony 8, Domain-Driven Design
- **Frontend**: Twig + HTMX (progressive enhancement)
- **Workers**: Go (async jobs, notifications, ML pipeline)
- **Database**: PostgreSQL with per-user schema isolation
- **Infrastructure**: Docker / Kubernetes (Minikube for local dev)
- **CI/CD**: GitHub Actions

## Privacy & GDPR

Health data is sensitive data (GDPR Art. 9). Grierson is privacy-first:
- Explicit consent on registration
- Data encrypted at rest (PII columns)
- Right to erasure built into the domain model
- No third-party analytics on health data

## Status

🚧 Active development — Phase 0 (scaffolding)

## License

MIT
