# GEO skill: where it came from

Copied on 2026-11-28 from https://github.com/zubair-trabzada/geo-seo-claude
(MIT license, see LICENSE in this folder). Reviewed before copying: the Python
scripts only make read-only GET requests to the site being audited and to public
pages (Wikipedia, Wikidata, Reddit, YouTube and similar) for brand checks. No
API keys, no hooks, nothing sends data anywhere.

Changes from upstream:
- Paths changed from `~/.claude/skills/geo/...` to `.claude/skills/geo/...` so the
  skill runs from this repo without the installer.
- Left out `geo-update` (it pulls new, unreviewed code from upstream and runs pip).
- Left out the agency sales layer: `geo-prospect`, `geo-proposal`, `geo-compare`,
  the Flask CRM web app and white-label config.
- Left out install/uninstall scripts, examples, tests and docs.

Python scripts need: `pip install -r .claude/skills/geo/requirements.txt`
(in a virtualenv). The `/geo report-pdf` command also needs pandoc and Chrome.

Reports (GEO-*.md) are written to the repo root; move them into `seo/` to keep.
`.vercelignore` keeps them off the live site.
