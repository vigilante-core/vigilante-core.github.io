# Vigilante Core — Hosted Console

**Live demo:** https://vigilante-core.github.io/

This repository hosts the static analyst console for the Vigilante defensive SOC MVP. It opens in clearly marked demo mode with synthetic events. The Pages site does not run an API, store customer data, authenticate users, ingest telemetry, or execute response actions.

To use real alerts and cases, deploy the backend from [saadcyber21/vigilante-core](https://github.com/saadcyber21/vigilante-core) on infrastructure you control, expose its API through HTTPS, set its `CORS_ORIGINS` to `https://vigilante-core.github.io`, then use **Connect API** in the dashboard. Never commit credentials, API tokens, or webhook secrets here.

The backend is a single-deployment MVP. Triage uses deterministic rules, not a trained AI model. Response proposals and approvals are records for human review only; no action is executed automatically. See the backend repository for setup, security, deployment, and scope documentation.

GitHub Actions publishes `docs/` to GitHub Pages when changes are merged to `main`.
