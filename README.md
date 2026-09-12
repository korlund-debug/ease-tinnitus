# EaseTinnitus

Sound therapy and self-guided tools that help many people manage tinnitus.

**Live:** https://ease.npgsystems.ca

EaseTinnitus is a small, installable web app (PWA) with three self-guided tools:

- **Pitch & Loudness Match** — a 4-step self-test to find the tone that best matches your tinnitus.
- **Sound Therapy** — white noise, pink noise, a personalized notched noise, and ocean-wave-like sound,
  generated live with the Web Audio API (no audio files, works fully offline).
- **Residual Inhibition Test** — a short listening session (1–30 min) some people use to temporarily
  quiet their tinnitus, with a quick before/after check-in.

## What this is (and isn't)

This is an independent, original wellness project. It is **not a medical device**, does not diagnose or
treat any condition, and is not affiliated with any hospital, clinic, or commercial audiology product.
See `about.html` in the app for the full safety notes.

## Running it

It's static HTML/CSS/JS with no build step and no backend:

```
# from this folder
npx serve .
# or just open index.html in a browser
```

All user data (matched pitch/loudness, session history) is stored only in `localStorage` on the user's
own device — nothing is sent to a server.

## Tech

Vanilla HTML/CSS/JS, Web Audio API for all sound generation, a manifest + service worker for
installable/offline PWA behavior (network-first, cache fallback).

## License

All rights reserved — see [LICENSE](LICENSE). The source is public for reference, but redistribution,
modification, or reuse is not permitted without permission from the copyright holder.
