# TheCatsizerLab portfolio

Portfolio website for https://thecatsizerlab.github.io/

GitHub Pages settings: `main` branch, `/ (root)`.

## Municipal portal

Valmer-sur-Rive is an independent fictional municipal demonstration at `/demos/municipal-website/`, with its case study at `/projects/municipal-portal.html` and complete FR/EN/ES/IT/DE versions of the portfolio, all ten case studies and the portal. English portfolio URLs stay at `/`; French municipal URLs stay at `/demos/municipal-website/`. Other languages use explicit locale paths.

Run `npm run build:i18n` after changing the shared renderers or editorial seed. Run `npm run test:municipal` for the core domain checks. Serve the repository root with any static HTTP server; no runtime dependencies or API keys are required.

The administration and citizen journeys use browser-local simulation data, without authentication, real transmissions or shared storage. Architecture, deployment, visual sources and verification results are documented in [docs/municipal/technical-guide.txt](docs/municipal/technical-guide.txt) and [docs/municipal/verification.html](docs/municipal/verification.html).

Internationalisation architecture, direct language URLs and measured QA results: [docs/i18n/verification.html](docs/i18n/verification.html). Translation sources are in `tools/i18n/`; runtime modules and compiled catalogues are in `assets/i18n/`. Python Beautiful Soup is required for the full static build, but not for the deployed website.

## Studio redesign

The portfolio presentation and case-study shell were redesigned on 26 November 2026. Run `python tools/i18n/build.py --portfolio-only` to rebuild the five-language portfolio without regenerating municipal pages. Python, Beautiful Soup and Pillow are build-time dependencies; the published site remains static. New editorial translations live in `tools/i18n/portfolio-studio.tsv`. See [measured verification](docs/studio/verification.html).
