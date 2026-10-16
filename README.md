# RCM Demo — AR Outlook

A healthcare revenue-cycle (RCM) analytics demo dashboard, covering:

- **AR Outlook** — AR aging by bucket, follow-up backlog, Day 45 liquidation trend, payer breakdown, and monthly driver trend
- **Denial Collectibility** — which denial category / payer / CPT combinations are most collectible (resolved-and-paid $ ÷ denied $), with a category × payer × CPT drill-down
- **A/R Rep Productivity** — team and per-rep daily productivity vs. target, and a leaderboard ranked by denial resolution success rate

This is a fully static, self-contained export (no backend required) — all data lives in `data/*.json` and is loaded client-side. All figures are synthetic sample data modeled to tell a coherent story, not real patient or claims data.

## Running locally

Any static file server works, e.g.:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080/`.

## Hosting

Push to GitHub Pages: **Settings → Pages → Deploy from a branch → `main` / `(root)`**.
