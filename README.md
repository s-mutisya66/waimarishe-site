# Waimarishe Kenya Ltd — Website

A single static page (`index.html`) — no build step needed.

## Deploy to Vercel (no domain yet)

**Option A — Vercel CLI (fastest, no GitHub needed)**
1. Install the CLI: `npm install -g vercel`
2. From this folder, run: `vercel`
3. Follow the prompts (log in / create account, confirm project settings, accept defaults).
4. Vercel gives you a live URL like `waimarishe.vercel.app` — that's your site, live.
5. Run `vercel --prod` to push it to the permanent production URL instead of a preview link.

**Option B — GitHub + Vercel dashboard**
1. Push this folder to a new GitHub repo.
2. Go to vercel.com → New Project → import the repo.
3. Framework preset: "Other" (it's plain HTML, no build command needed).
4. Deploy — you'll get a `.vercel.app` URL immediately.

Either way, every time you push a change (or run `vercel --prod` again), the live site updates.

## Later: adding your own domain
Once you're ready, buy `waimarishekenya.co.ke` (or similar) through a registrar, then in the Vercel
project settings go to **Domains** and add it — Vercel gives you the exact DNS records to paste into
your registrar.

## Note on the contact form
The form currently just shows a placeholder confirmation — it isn't wired to send anywhere yet.
Easiest options once you're ready:
- **Formspree** or **Web3Forms** — drop-in form backends, no server code needed.
- A Vercel Serverless Function that emails you or writes to a database.
