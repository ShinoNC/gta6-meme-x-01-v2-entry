# gta6-meme-x-01 — LEONIDA AIRLINES: DELAYED 13 YEARS

[![make.fun · gta6-meme-x-01](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![rank](https://make.fun/badge/gta6-meme-x-01/ShinoNC/gta6-meme-x-01-v2-entry/rank.svg)](https://make.fun/bounty/gta6-meme-x-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![reward](https://make.fun/badge/gta6-meme-x-01/ShinoNC/gta6-meme-x-01-v2-entry/reward.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)

An entry for make.fun's bounty **"Post a GTA 6 meme on X"** ($500, top 50 paid).
The post itself is the entry: an AI judge compares the posts two at a time.

make.fun is a site where people and their AI agents build things, enter them in
paid competitions (bounties) and earn real money when they win.

## The meme

![LEONIDA AIRLINES boarding pass: Los Santos to Vice City, delayed 13 years.](meme.png)

A boarding pass for the longest flight in gaming: **LEONIDA AIRLINES,
flight VI-2013, Los Santos → Vice City.** Departed September 17, 2013 (the
day GTA V came out); arriving November 19, 2026 (the day GTA VI came out) —
stamped **DELAYED 13 YEARS**. Every line on the pass is a launch-week joke
built on a real fact:

- **GATE A1 → B2 → C6** — the gate changed twice, like the release date.
- **SEAT 13A, CLASS: PATIENCE** — the only class this flight sells.
- **CARRY-ON: 214 GB** — the real pre-load size; **CHECKED: FAMILY PHOTOS —
  DELETED TO MAKE ROOM** — what the download actually cost.
- **FARE $79.99** — the real standard-edition price, **PAID BY MY AI AGENT**
  with a bounty payout it earned on make.fun. The make.fun ghost rides the
  pass twice: as the airline's roundel logo and 350px tall in the payment
  band.
- **"Please keep this pass. The 13-year wait is non-refundable."**

## How it is made

`meme.html` (HTML/CSS/SVG, all text rendered in code) is screenshotted to
`meme.png` at 1024×1024 by `render_meme.py` (headless Chromium via
Playwright). Two runs produce byte-identical output. The ghost is the
official make.fun mark from the press kit. No Rockstar logos or artwork,
no copyrighted characters. `main.ts` copies `POST.json` (the X post's
address) to the output directory.

## The post

The user posts `meme.png` from their own public X account with the caption
in `CAPTION.txt`, then `POST.json` is updated with the real post URL before
submitting.
