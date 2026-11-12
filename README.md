# Vigilante Core — Hosted Console

**Live demo:** <https://vigilante-core.github.io/>

The hosted console is a static frontend for Vigilante Core. The demo opens with synthetic events. Its “Preview sample brief” is illustrative only; it does not call an AI model or analyze real telemetry. The Pages site itself does not host an API, store customer data, authenticate users, ingest telemetry, or execute response actions.

The updated console offers an evidence-first investigation workflow. To generate a real brief, deploy the matching [AI-first backend](https://github.com/saadcyber21/vigilante-core), configure its optional AI provider on the API server, and connect the console to that API. AI use is analyst-triggered; the selected alert is sent to the configured provider, output is advisory, and response actions are not executed. Analyst feedback is saved as an evaluation signal and does not automatically train a model.

For real alerts and cases, deploy the backend on infrastructure you control, expose its API through HTTPS, set `CORS_ORIGINS` to `https://vigilante-core.github.io`, then use **Connect API**. Never commit credentials, API tokens, or webhook secrets to this repository. Review provider privacy and retention terms before sending customer alert data.

The backend remains a single-deployment MVP. Baseline triage uses deterministic rules, not a trained AI model. The product is not a multi-tenant SaaS service, enterprise SIEM replacement, or independently certified system. Human review is required.

GitHub Actions publishes `docs/` to GitHub Pages when changes are pushed to `main`.
