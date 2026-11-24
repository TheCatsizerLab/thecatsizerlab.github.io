# TheCatsizerLab portfolio

Portfolio website for https://thecatsizerlab.github.io/

GitHub Pages settings: `main` branch, `/ (root)`.

## Municipal portal

Valmer-sur-Rive is an independent fictional municipal demonstration at `/demos/municipal-website/`, with its case study at `/projects/municipal-portal.html` and a French portfolio overview at `/fr/`.

Run `npm run build:municipal` after changing the shared renderers or editorial seed. Run `npm run test:municipal` for the core domain checks. Serve the repository root with any static HTTP server; no runtime dependencies or API keys are required.

The administration and citizen journeys use browser-local simulation data, without authentication, real transmissions or shared storage. Architecture, deployment, visual sources and verification results are documented in [docs/municipal/technical-guide.txt](docs/municipal/technical-guide.txt) and [docs/municipal/verification.html](docs/municipal/verification.html).
