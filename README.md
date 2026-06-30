# Procedural Music Generator

A browser-based procedural music generator: chord progressions, modal scales, multi-voice arrangement (melody/bass/harmony/drums), per-voice synth timbres, and a live mixer — all running client-side with [Tone.js](https://tonejs.github.io/).

🔗 **Live site:** `https://<your-username>.github.io/<repo-name>/`

## Before you launch

`index.html` has placeholder Open Graph URLs (`YOUR-USERNAME`/`YOUR-REPO`) — once you know your live URL, find-and-replace those with your actual GitHub Pages URL so link previews (Discord/Slack/Twitter) point to the right place and pick up `og-image.png`.

## Running locally


No build step. Just open `index.html` in a browser, or serve it:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying

This repo is set up for GitHub Pages — see the deployment steps in the project notes, or just push to `main` and enable Pages in repo Settings → Pages → Source: `main` / root.

## Tech

- Single static HTML file, no build pipeline
- [Tone.js](https://tonejs.github.io/) (loaded via CDN) for audio synthesis/scheduling
- Presets saved to browser `localStorage`
