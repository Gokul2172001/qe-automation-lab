# QE Automation Lab

A quality engineering platform built in public with **n8n, Jenkins, Playwright, PostgreSQL, Grafana and local AI**.
n8n orchestrates, other tools execute, and Postgres remembers every run.

> **Status: v0.0, repo scaffolded.** Nothing runs yet. Follow the progress below.

## What this project is

An end-to-end lab that:
- triggers API and UI test suites automatically,
- stores every result in a database,
- raises defects and alerts when tests fail,
- shows quality trends on a dashboard,
- uses AI to analyze failures and triage bugs.

Everything runs locally with free and open-source tools.

## Architecture

See [docs/architecture.md](docs/architecture.md). The diagram grows as services are added.

## Roadmap

- [ ] **v0.1** Base stack: Docker, Postgres, n8n
- [ ] **v0.2** First workflow: webhook to database
- [ ] **v0.3** Jenkins triggers tests and calls n8n
- [ ] **v1.0** Project 2: API testing platform
- [ ] **v1.1** Project 4: UI regression orchestrator
- [ ] **v1.2** Project 6: Synthetic monitoring
- [ ] **v1.3** Project 9: Quality metrics dashboard (Grafana)
- [ ] **v2.0** Project 3: AI failure analysis
- [ ] **v2.1** Project 1: AI test case generator
- [ ] **v2.2** Project 5: Bug triage and duplicate detection
- [ ] **v3.0** Release-readiness platform

## Tech stack

| Area | Tool |
|---|---|
| Orchestration | n8n |
| CI | Jenkins |
| UI tests | Playwright |
| API tests | UI Tests | Playwright |
| Database | PostgreSQL (+ pgvector) |
| Dashboards | Grafana |
| AI | Ollama (local LLMs) |
| Defect tracking | GitHub Issues |
| Containers | Docker Compose |

## Skills progress

| Skill | Start | Now | Evidence |
|---|---|---|---|
| Docker | Beginner | Beginner | - |
| PostgreSQL / SQL | None | None | - |
| n8n | Beginner | Beginner | - |
| Jenkins | None | None | - |
| Playwright | - | - | - |
| Grafana | None | None | - |

The "Now" column is only updated when there is evidence (a commit, project or write-up).

## Repository layout

```
infra/           database init scripts, service configs
n8n-workflows/   exported workflow JSON
projects/        one folder per project, each with its own README
docs/            architecture, learning log, screenshots
```

## Getting started

Setup instructions will be added in v0.1.

## Documentation

- [Changelog](CHANGELOG.md)
- [Learning log](docs/learning-log.md)
- [Parking lot](docs/parking-lot.md)
- [Docker and Git cheat sheet](docs/cheatsheets/docker-git-cheatsheet.pdf)
## License

MIT