# Mark R. Routson — Product Delivery Portfolio

A static portfolio site describing selected product and delivery work, with screenshots.
**No source code from any of the described systems is included in this repository** — this is a
description of work, not a distribution of it.

**Live site:** enable GitHub Pages (below), then visit `https://<your-username>.github.io/<repo-name>/`

## What's here

```
index.html            single self-contained page (all CSS/JS inline)
img/soar/              8 screenshots — SOAR forecasting platform
img/wastewater/        4 screenshots — Wastewater Early Warning System
img/competitive/       4 screenshots — Platform Scorecard (scores, rubric, radar, detail)
img/portfolio/         2 screenshots — Portfolio Impact Dashboard
img/burden/            1 screenshot  — Burden & Demand Model
img/genomics/          1 screenshot  — SARS-CoV-2 world map
img/rmse/              1 screenshot  — Forecast hub RMSE
img/efv/               1 photo       — Expeditionary Fighting Vehicle (USMC, public domain)
.nojekyll             tells GitHub Pages to serve files as-is
```

22 images, ~4 MB total. Sections are ordered so the visual case studies lead. Inventory and Alert Center screens are deliberately withheld as
proprietary — those two case studies carry their capability description only.

## Contents of the site

| Section | Covers |
|---|---|
| About | Bio, contact details, certifications — placed before the case studies |
| Vexus overview | Platform, state health department rollout, forecast → alert → response |
| Case study 01 | SOAR — forecasting, MQAT, ensemble builder, UShER, lab results, alerts, measles |
| Case studies 02–05 | Wastewater; Burden & Demand Model; SARS-CoV-2 world map; Forecast hub RMSE |
| Case studies 06–07 | Platform Scorecard (competitive analysis); Portfolio Impact Dashboard |
| Case study 08 | Expeditionary Fighting Vehicle — General Dynamics, IT/M&S IPT Lead |
| Case studies 09–10 | Inventory & Supply Chain; Alert Center — text only, screens withheld |
| Case studies 11–13 | Pertussis SEIRS model, spend-plan AI validation harness, mobile PWA |
| Method | AI-assisted delivery measured across five modules (1,160 hrs est → 182 hrs actual) |

## Publishing to GitHub

```bash
cd portfolio
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Then in the repo: **Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)` → Save.**
The site is live in a minute or two.

To preview locally first:

```bash
python -m http.server 8000     # then open http://localhost:8000
```

## Before you publish — please review

- **Employer clearance.** The screenshots are of a proprietary product built for an employer.
  Confirm you're cleared to publish product UI publicly.
- **Portfolio screens use the dashboard's default demo book** (MSFT, AAPL, TSLA, META, AMZN, NVDA) —
  not your real positions. Nothing personally financial is exposed.
- **SOAR screens come from the published user guide** — demonstration data and sample IDs, no PHI.
- **Wastewater and burden screens show public data.** The wastewater views render CDC NWSS and
  WastewaterSCAN open surveillance data, and the Burden & Demand Model shows Oregon 2025–26 planning
  defaults — all public sources, nothing customer-confidential.
- **Scorecard names are anonymized** to "Acme"; competitor names shown are public products.
- **The EFV photo is a U.S. Marine Corps image in the public domain** (US federal government work),
  sourced from Wikimedia Commons. It links out to a video of the vehicle.
- **Customer naming.** The site deliberately describes customers generically ("a state department of
  public health", "a federal forecasting center"). Swap in real names only if you have permission.

## Editing

Everything is in `index.html` — one file, no build step, no dependencies. Content sections are
commented and each case study is a `<article class="case">` block you can copy to add another.
