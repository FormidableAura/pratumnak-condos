# Pattaya Living — the condo shortlist

**Live page:** https://formidableaura.github.io/pratumnak-condos/

The current page (v4, deployed 30 Oct evening) is a **city-wide** shortlist:

- All Pattaya + neighbourhood chips (Pratumnak, Central, North, South, Jomtien, Wongamat, East)
- Default: ≤ **฿19,000/mo** · ≥ **25 m²** · condos only · 6-month-friendly (confirmed
  1-year-only units hidden behind the Contract chip) · **cheapest first**
- **63 condos** match the default set (129 gathered city-wide) — every row links to its
  original advert and shows its source
- Benchmark: the owner's current 64 m² at ฿14,000 = **฿219/m²**, displayed as "The value to beat"

Sources: Facebook Marketplace (anonymous), Rightmove Pattaya, Alan Bolton Property, and
Central City Property (the letting agent — its terms block is authoritative where stated).
Photos belong to the listings. Prices are asking rents; lease terms only where an agent
states them.

- `index.html` + `images/` — the live page (plain HTML/CSS/JS)
- `listings.json` — the dataset (140 records incl. off-brief); `parse_all.py` regenerates it
- `refresh.py` — Rightmove live refresh; `build.py` — page build; `deploy.sh` — push to Pages
- `requirements.md` — the brief as it grew (v1 floor → v4 19k cap, plus the handover manifest)

## Branches
- `backup-live` — the interim Pratumnak Soi 4–6 page kept by the 30-Oct evening research
  pass (`git checkout backup-live -- .` to restore)

## Notes
- TWO agent sessions wrote to this repo on 30 Oct. If a push ever reports non-fast-forward:
  `git pull --rebase`, resolve `index.html` to the current build, re-push. The other
  session's replacement page is preserved on `backup-live`.
- Facebook Marketplace is IP-gated for anonymous browsing (since 30 Oct evening) — resume
  per the marketplace-harvesting skill pacing rules, don't hammer.
- A daily 10:00 cron re-harvests and redeploys this page when Rightmove changes.