# Spruce Knowledge Base (`spruce-kb`)

Public educational knowledge base for a **defined-risk options** operating process.

**Not financial advice.** Nothing in this repo is a recommendation to buy, sell, or hold any security. Verify brokerage, tax, and account rules with your broker and qualified advisors (including CRA where relevant).

## What this is

- Curriculum and playbooks for credit spreads (PCS / CCS), risk policy drafts, and Canadian retail notes
- Companion private ops tooling is **out of scope** for this repo

## Two builds

| Build | Command | Includes |
|-------|---------|----------|
| **Local / full** | `mkdocs serve` | Curriculum + private operator pages (open decisions, migration tracker, verification log) |
| **Public (Pages)** | `mkdocs serve -f mkdocs.public.yml` | Curriculum only — no personal decision log, migration tracker, or private verification notes |

```bash
cd spruce-kb
pip install -r requirements.txt
mkdocs serve -f mkdocs.public.yml   # what GitHub Pages deploys
```

Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

Suggested reading order: [How to use this site](docs/00-meta/how-to-use-this-site.md).

## GitHub Pages

On push to `main`, [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml) builds with **`mkdocs.public.yml`** and deploys to GitHub Pages.

**First-time setup:** Repo → Settings → Pages → Build and deployment → Source: **GitHub Actions**, then re-run the workflow.

## License

Apache License 2.0 — see [LICENSE](LICENSE) and [NOTICE](NOTICE).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).
