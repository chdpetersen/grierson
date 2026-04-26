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

## Roadmap

### Phase 0 — Scaffolding *(current)*
- [ ] Symfony 8 project setup with DDD folder structure
- [ ] Docker Compose for local development
- [ ] Minikube setup with `grierson-dev` namespace
- [ ] GitHub Actions: lint + unit tests on push

### Phase 1 — MVP: Auth & Appointments
- [ ] User registration with explicit GDPR consent flow
- [ ] Health profile setup
- [ ] Appointment scheduling with medical specialties
- [ ] Email reminders
- [ ] Unit tests for `Appointment` bounded context

### Phase 2 — Medical Records
- [ ] Document and study upload (PDF, images)
- [ ] Unified health timeline per user
- [ ] PII column encryption (Doctrine Extensions)
- [ ] REST API with OpenAPI/Swagger documentation
- [ ] Go worker: async file processing

### Phase 3 — Cycle & Wellbeing
- [ ] Menstrual cycle tracking with symptom logging
- [ ] Emotional wellbeing journaling
- [ ] Basic correlations: symptoms × cycle × appointments
- [ ] Cloud Kubernetes deployment (Helm charts)

### Phase 4 — AI Layer
- [ ] Anonymised longitudinal data export pipeline
- [ ] LLM integration for personalised health insights
- [ ] Pattern detection and preventive alerts
- [ ] Granular consent panel for AI data usage

---

## Contributing

Grierson is in early development and welcomes contributors.

### How to contribute

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes following [Conventional Commits](https://www.conventionalcommits.org/)
4. Open a Pull Request with a clear description of what and why

### What we're looking for

- Bug reports and fixes
- Improvements to the DDD domain model
- Additional test coverage
- Translations (the platform targets a global audience)
- UX feedback on health data flows

### Guidelines

- All health data handling must comply with GDPR Art. 9 (sensitive data)
- New features should include unit tests for domain logic
- Follow PSR-12 for PHP code style
- Keep PRs focused — one concern per PR

### Code of Conduct

This project is committed to providing a welcoming and inclusive environment.
All contributors are expected to uphold respectful and constructive communication.

### Questions?

Open an issue or start a discussion in the [GitHub Discussions](https://github.com/chdpetersen/grierson/discussions) tab.
