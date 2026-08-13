# Contributing to Spruce KB

Thank you for interest in improving Spruce. This knowledge base is educational and operator-facing.

## Editorial standards

- **No personalized advice.** Do not tell readers what to buy, sell, or hold for their situation.
- **No live trade calls.** Do not publish “trade this now” content or real-time signals.
- **Anonymized examples only.** Never include real account numbers, identifiable portfolio sizes, or unscrubbed fills.
- **Tag claims.** Prefer `[verified]`, `[personal preference]`, or `[pending-verify]` / `[course-derived]` on numeric or rule-like claims.
- **Disclaimer-first.** Keep the site-wide disclaimer intact; section footers may reinforce it.

## How to contribute

1. Open an issue describing the change (typo, clarification, new page outline).
2. Prefer small PRs that map to existing taxonomy pages under `docs/`.
3. Run `mkdocs build -f mkdocs.public.yml --strict` locally before opening a PR.
4. Do not commit secrets, portfolio exports, or broker credentials.

## Farsi translations

Public pages have a Farsi sibling: `page.md` (English) and `page.fa.md` (Farsi). English stays at `/`; Farsi at `/fa/`.

- Translate prose, headings, and explanations.
- Keep glossary **term names** and technical terms in English (Call, Put, Delta, PCS, credit spread, TFSA, and so on).
- Keep markdown link targets without a `.fa` suffix (`glossary.md`, not `glossary.fa.md`).
- Keep formulas, tickers, dollar amounts, tags (`[verified]`, …), and bash commands unchanged.
- Private operator pages may stay English-only; the build falls back to the English file.
- Farsi UI/body type is VazirMatn; do not switch Farsi pages to another family.

## Voice

Educational, operational, non-advisory. Prefer checklists and playbooks over hype.

## Ownership

CODEOWNERS / sole owner initially: Mohammad.
