# Artist Mutual Aid Directory 🦋
### Open-source resource directory for BIPOC and LGBTQ+ artists

**[→ View the Live Directory](https://jiandamonique.github.io/google-kaggle-mutual-aid-artist/)**

> *"Each one, reach one. Each one, teach one."*

---

## What This Is

A curated, searchable directory of mutual aid resources for BIPOC and LGBTQ+ artists — housing, healthcare, grants, direct financial aid, legal support, and community networks.

Built with vanilla HTML, CSS, and JavaScript. No framework. No server. No cost to host. The whole site is one file you can open in a browser, zip and share, or fork and make your own.

This is more than a landing page — it is a living iteration hub and archive for a development journey built in public. As a restorative justice creative, I believe in transparency and growth, which is why every version, milestone, and pivot of this project is documented here. The roadmap is honest. The process is the work.

---

## Use This For Your Community

This project is designed to be forked. If you run a mutual aid network, artist collective, community organization, or resource hub — you can take this codebase and make it yours.

**To fork it:**

1. Click **Fork** in the top right corner of this repo
2. Replace the resource data in `index.html` with your own (it's a simple JavaScript array near the bottom of the file)
3. Update the colors, category names, and copy to fit your community
4. Enable GitHub Pages in your repo settings — your directory is live

**Need help?** Open an [Issue](https://github.com/jiandamonique/google-kaggle-mutual-aid-artist/issues) and describe what you're trying to build. I'll help you get set up.

Zero technical background required to ask. That's the point.

---

## Features

- **Live search** — filters by name, description, tags, and eligibility as you type
- **Category filters** — Housing, Healthcare, Grants, Direct Aid, Legal, Community, Mutual Aid
- **Tab navigation** — Directory and About in one lightweight page
- **Fully responsive** — works on mobile, tablet, desktop
- **Zero dependencies** — no npm, no build step, no server needed
- **Forkable and zippable** — the whole site travels in one HTML file

---

## Data Sources

The original 2021 plan assumed bulk public datasets (NEA/arts.gov exports, scraped directories, broad search via Kaggle and Google's filetype search) would supply most of the directory's content. That landscape has changed. Bulk dataset search has gotten significantly harder since 2021 — search engines deprioritized raw file-type queries, several previously reliable sources turned out to be inconsistent or no longer maintained, and platforms like Kaggle are built for competition-ready ML data, not niche civic/social-service directories.

So the approach has shifted: **this directory is now built on manually vetted data**, not bulk import. Every resource listed has been individually researched and verified — slower, but more accurate, and arguably more honest about what a small, independent mutual aid project can realistically maintain.

| Source | Method | Status |
|--------|--------|--------|
| Sample data | Curated placeholder entries across all 7 categories, manually researched | Launched |
| Community submissions | Submitted via the site's "Submit a Resource" tab, reviewed before inclusion | Live |
| Manually vetted additions | Individually researched and added over time as capacity allows | Ongoing |
| NEA / arts.gov | Originally planned as a bulk source — found unreliable on review | Deferred |
| MutualAidHub | Originally planned as a bulk source — no clean export available; usable as a manual reference | Deferred |
| 211.org API | Still a possible future integration if API access becomes feasible | Future / Unconfirmed

This is a smaller, slower path than the original 2021 plan — and it's the realistic one. Manual curation is re-injected back into the process due to data availability shifts.Will ramp back up to automation.

---

## Origin

This project was born during the **2021 Kaggle/Google BIPOC Data Fellowship**, mentored by [Prasun Kumar Mishra](https://www.kaggle.com/prasunmishra) and [Julia Elliott](https://www.kaggle.com/juliaelliott).

**2021 Foundation** — The original data architecture, pipeline design, and research built during the fellowship. ~100 datasets identified. A Python → BeautifulSoup → Pandas → Jekyll pipeline designed. The vision written down.

**2026 Revival** — The modern, iterative push to bring the Artist Mutual Aid Directory to life using zero-dependency, foundational web technologies. Same roots. Deeper commitment.

The fellowship sparked the idea. Life interrupted. In 2026, the project was revived alongside a published novel ([*My Beautiful Device*](https://books2read.com/mybeautifuldevice)) that shares the same mission: what it means to need help, ask for it, and keep going when the system isn't built for you.

The full story: [Oversharing What's Overlooked](https://jiandamonique.medium.com/oversharing-whats-overlooked-3ef8c0a4a52b) — the original fellowship blog post.

---

## Roadmap

- [x] Prototype directory built — sample data, all 7 categories, live search and filters
- [x] Single-page tab navigation — lightweight, zippable
- [x] Project continuity documented — discussion of hiatus from 2021 to 2026
- [x] Update all repo descriptions
- [ ] Continue to integrate data
- [ ] Build out artist-specific resource sections

---

## Repositories

| Repo | Purpose |
|------|---------|
| [google-kaggle-mutual-aid-artist](https://github.com/jiandamonique/google-kaggle-mutual-aid-artist) | This repo — live directory |
| [kaggle-google-mutual-aid-devpage](https://github.com/jiandamonique/kaggle-google-mutual-aid-devpage) | Back end archive and dev hub |
| [google-kaggle-mutual-aid-artist.github.io](https://github.com/jiandamonique/google-kaggle-mutual-aid-artist.github.io) | Archived 2021 Jekyll fellowship site |
| [Google Drive — Project Archive](https://drive.google.com/drive/u/1/folders/1QodJ016_nw7tzJJ9T8KN6AYhJN0JRI_P) | Planning worksheets, dataset research, milestone tracking, and fellowship documentation — the origin of the project |

---

## Support This Work

This is an unfunded, independent project. If the vision resonates — a forkable, community-owned mutual aid infrastructure anyone can use — any support helps keep it going.

- 💸 [Venmo](https://venmo.com/jayevajohnson)
- 💳 [PayPal](https://www.paypal.com/paypalme/jmcommunity)
- ❤️ [GoFundMe](http://www.gofundme.com/f/help-me-develop-artist-mutual-aid-site)

---

## Contributing

Found a broken link? Know a resource that should be here? Want to help with data integration?

Open an [Issue](https://github.com/jiandamonique/google-kaggle-mutual-aid-artist/issues) or submit a Pull Request. All contributions welcome — code, data, or just flagging something that needs fixing.

---

## Connect

- ✍️ [Origin Story — Medium](https://jiandamonique.medium.com/oversharing-whats-overlooked-3ef8c0a4a52b)
- 🌐 [Portfolio](https://jiandamonique.github.io)
- 💼 [LinkedIn](https://www.linkedin.com/in/jiandamonique)

---

*Open source · MIT License · Built in public · Art heals. Code connects. Each one, reach one.*
