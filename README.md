# Vigilante Core — Community SOC Console

This repository hosts the static web console for the open-source Vigilante security operations project.

**Live site:** https://vigilante-core.github.io/

The console opens in clearly labeled demo mode with synthetic events. It does not ingest telemetry, store alert data on a server, or run the API. To view live alerts and cases, deploy the backend from [saadcyber21/vigilante-core](https://github.com/saadcyber21/vigilante-core) separately, expose it over HTTPS, configure its `CORS_ORIGINS` to include `https://vigilante-core.github.io`, then connect it from the dashboard. Never place API or webhook secrets in this static repository.

GitHub Actions publishes the contents of `docs/` to GitHub Pages on pushes to `main`. The backend and deployment instructions remain in the linked source repository.
