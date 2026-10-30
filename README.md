# Pratumnak Hill condo shortlist

A live-updating shortlist of rental condos on Pratumnak Hill, Pattaya — filtered to the
brief (≤ ฿16,000/mo · 25 m²+ · 6-month-friendly · condos only) and sorted by the space
each baht buys (฿/m²), benchmarked against the owner's current 64 m² at ฿14,000.

**Live page:** https://formidableaura.github.io/pratumnak-condos/

Sources: Facebook Marketplace (anonymous, no account), Rightmove Pattaya, and Alan Bolton
Property Consultants. Photos belong to their listings. Prices are asking rents.

- `index.html` + `images/` — the page (plain HTML/CSS/JS, no build step)
- `listings.json` — the dataset; `parse_all.py` regenerates it from raw harvests
- `refresh.py` — live refresh from Rightmove over plain HTTP (cron)
- `deploy.sh` — pushes the current build to Pages
- `requirements/see requirements.md` — the brief as it grew