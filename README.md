# Pratumnak Soi 4-6 condo shortlist

**Live page:** https://formidableaura.github.io/pratumnak-condos/

Brief: rental condos at/between Pratumnak Soi 4 and Soi 6, Pattaya — long-term asks
≤ ฿16,000/mo, price-sorted and soi-labeled. Hunted 30 Oct 2026 across Alan Bolton
Property Consultants (pattaya-property.net), East Coast Real Estate (thaiproperty.com)
and listing portals (Hipflat, FazWaz, RenThai, BahtSold, PropertyHub, inpattaya.net).
Every card carries its source link, freshness stamps, and ⚠ caveats for undated/older
listings.

- `index.html` — the live page (plain HTML/CSS, no build step)
- branch `backup-live` — the previous richer snapshot (13:58 harvest: Rightmove/ABPC/
  Facebook Marketplace photos, m²-sorted layout) — restorable with
  `git checkout backup-live -- .`

Refresh procedure: re-harvest, replace `index.html`, push to `main`; keep a backup
branch before overwriting anything. Facebook Marketplace was IP-gated for anonymous
browsing on the evening of 30 Oct — resume it next session (marketplace-harvesting
pacing rules), don't hammer.