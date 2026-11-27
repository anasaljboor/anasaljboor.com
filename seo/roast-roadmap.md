# SEO roast roadmap: anasaljboor.com (2026-11-27)

Verdict: Google can crawl you fine, but the page was written for recruiters, so it had nothing a client could search for or act on.

Checks run against the live site from a browser on 2026-11-27: `/` 200, `/robots.txt` 200 (allow all, sitemap listed), `/sitemap.xml` 200 XML, `/no-such-page-xyz` 404 (no soft 404), `/.claude/settings.json` and `/README.md` 404 (agent files are not served). No ranking or traffic data was available (no Search Console or Ahrefs access), so the keyword choices below are informed guesses until Search Console data comes in.

| # | Tier | Issue | Revenue impact | Fix | Owner | Status |
|---|---|---|---|---|---|---|
| 1 | REVENUE | Title, H1 and description targeted "Full-Stack & DevOps Engineer", a job title people search when hiring, not when buying | Clients searching "web developer Amman" or "DevOps consultant Jordan" never see the page | Title, H1, description and OG aligned on "Freelance Web Developer & DevOps Engineer" (Amman, Jordan in H1 and description) | agent | shipped in PR |
| 2 | REVENUE | No services, no process, contact said "open to roles" | Client visitors had no offer to evaluate and no reason to write | Four service blocks with scope and typical time, a four-step process, FAQ | agent | shipped in PR |
| 3 | REVENUE | Only contact path was mailto and LinkedIn | Visitors on phones without a mail app drop off | Contact form (Formspree, falls back to mailto until the form ID is set) | agent + Anas | shipped, form ID pending |
| 4 | REVENUE | JSON-LD described only a Person | Google and AI assistants could not tell the site sells services | `ProfessionalService` with offer catalog and service area, `WebSite`, `FAQPage` | agent | shipped in PR |
| 5 | COMPOUNDING | AI assistants have no summary to quote | ChatGPT, Perplexity and Claude answer "who can build X in Jordan" from other sources | `/llms.txt` with the same facts as the page | agent | shipped in PR |
| 6 | COMPOUNDING | Search Console and Bing Webmaster Tools not confirmed | No data on queries, clicks or indexing | Verify both, submit sitemap, request indexing after merge | Anas | next |
| 7 | COMPOUNDING | No Google Business Profile | Missing from Maps and "near me" results in Amman | Create a service-area profile (no public address needed) | Anas | next |
| 8 | COMPOUNDING | Few links point to the site | A one-page site with no links ranks only for its brand name | LinkedIn featured link, GitHub profile README, Clutch/GoodFirms/Upwork profiles, Jordanian and Gulf directories, guest posts (see blitz-plan.md) | Anas | next |
| 9 | COMPOUNDING | One page tries to rank for every service | Each service keyword competes with the others | After the blitz, split into `/web-development-jordan` and `/devops-consulting` pages, each linked from the home page | agent | after day 30 |
| 10 | COMPOUNDING | English only | Arabic searches ("مطور مواقع في الأردن", "تصميم مواقع عمان") go to competitors, and Gulf clients often search in Arabic | Add an Arabic version at `/ar/` with reciprocal hreflang, fully translated (no half-translated pages) | agent + Anas | decide |
| 11 | REVENUE | No photo, testimonials or client logos | Lower trust for first-time clients | Add a real photo; ask KOUN or past clients for a one-line quote they approve | Anas | next |

## Fluff (ignore until rows above ship)

- OG image still says "Full-Stack & DevOps Engineer"; regenerate it as "Freelance Web Developer & DevOps Engineer".
- Custom 404 page added in this PR (it was a plain-text Vercel 404).
