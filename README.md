# anasaljboor.com

Personal portfolio. Plain HTML + CSS, no build step — Vercel serves it as a static site.

## Edit content
All content is in `index.html`. Remaining TODO: CV at `/cv.pdf`; optional photo at `/me.jpg`, push, done.

## Run locally
```bash
python3 -m http.server 8080   # then open http://localhost:8080
```

## Deploy to Vercel
1. Push this folder to a GitHub repo.
2. vercel.com → Add New → Project → import the repo.
3. Framework preset: **Other**. Leave build command and output directory empty.
4. Deploy. Every push to `main` redeploys; every PR gets a preview URL.

## Custom domain (anasaljboor.com)
1. Project → Settings → Domains → add `anasaljboor.com` (Vercel will offer `www` too).
2. At your registrar's DNS:
   - `A` record, host `@` → `76.76.21.21` (or the value shown on the domain card)
   - `CNAME` record, host `www` → the CNAME target shown on the domain card
   - Delete any old `A`/`AAAA` records on `@` (registrar parking pages).
3. Pick one canonical host (apex or www) and let Vercel redirect the other.
4. SSL is issued automatically once DNS propagates. Check with `dig a anasaljboor.com`.
