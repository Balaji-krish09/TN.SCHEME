# TN.Scheme

An independent, open-source website that helps Tamil Nadu citizens figure out which government
welfare schemes they're actually eligible for — no jargon, no forms to dig through, just a short
guided Q&A that matches you to real schemes based on real eligibility criteria.

**This is not a government product.** It's a personal civic-tech project built to make publicly
available scheme information easier to act on.

## How it works

1. Pick who you are: Farmer, Health & Insurance, Student, Small Business Owner, or General Citizen.
2. Answer a few short questions about your situation (income, community category, land size, etc.
   — whatever that category's real schemes actually require).
3. Get matched to the specific schemes you qualify for, each with:
   - The official scheme link, up top
   - A plain-language summary and background (who introduced it, when, current status)
   - Who it's actually for
   - Documents required
   - How to apply

Every scheme's eligibility rules were sourced from official government pages, department portals,
or verified secondary sources. Where a detail couldn't be independently confirmed, the app says so
rather than guessing.

## Status

| Category | Status |
|---|---|
| Farmer | Live |
| Health & Insurance | Live |
| Student | Live |
| General Citizen | Live |
| Small Business Owner | Coming soon |

## Tech

Plain HTML/CSS/JS, no framework, no backend — scheme data lives in `data/schemes.json` and is
matched client-side against your answers. Built this way so it's easy to audit, fork, and extend.

## Running locally

Open `frontend/index.html` in a browser, or serve the repo root with any static file server so the
relative fetch to `../data/schemes.json` resolves correctly.

## Contributing

Found a scheme with outdated info, or want to help add the Small Business category? Open an issue
or a PR — corrections to eligibility criteria, income thresholds, or scheme links are especially
welcome since these change with government orders.
