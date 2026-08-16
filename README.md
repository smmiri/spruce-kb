# Spruce Knowledge Base (`spruce-kb`)

Public educational knowledge base for a **defined-risk options** operating process.

**Not financial advice.** Nothing in this repo is a recommendation to buy, sell, or hold any security. Verify brokerage, tax, and account rules with your broker and qualified advisors (including CRA where relevant).

## What this is

- Curriculum and playbooks for credit spreads (PCS / CCS), risk policy drafts, and Canadian retail notes
- Companion private ops tooling is **out of scope** for this repo

## Languages

The public site is bilingual. Use the header language switch:

| Locale | URL | Notes |
|--------|-----|-------|
| English (default) | `/` | Existing pages unchanged |
| فارسی | `/fa/` | RTL, VazirMatn; glossary term names and technical terms stay in English |

Farsi sources are sibling files (`page.fa.md` next to `page.md`). See [CONTRIBUTING.md](CONTRIBUTING.md).

## Local preview

```bash
cd spruce-kb
pip install -r requirements.txt
mkdocs serve
```

Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) (English) and [http://127.0.0.1:8000/fa/](http://127.0.0.1:8000/fa/) (Farsi).

Suggested reading order: [How to use this site](docs/00-meta/how-to-use-this-site.md).

## GitHub Pages

On push to `main`, [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml) runs `mkdocs build --strict` and deploys to GitHub Pages.

Canonical URL: **https://spruce.smmiri.com/**

**First-time setup (fixes `configure-pages` / site 404):**

1. Repo → **Settings → Pages** → Build and deployment → Source: **GitHub Actions**
2. Custom domain: `spruce.smmiri.com` (DNS below), then enable **Enforce HTTPS** when GitHub offers it
3. Re-run the workflow (Actions → Deploy to GitHub Pages → Run workflow)

### DNS (Cloudflare, zone `smmiri.com`)

| Type | Name | Target | Proxy |
|------|------|--------|-------|
| CNAME | `spruce` | `smmiri.github.io` | DNS only |

`docs/CNAME` is copied into the built site so GitHub keeps the custom domain on each deploy.

## License

Apache License 2.0 — see [LICENSE](LICENSE) and [NOTICE](NOTICE).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).
