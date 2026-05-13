# SynthNerd — Daily 60s Synth History

Live site: https://synthnerd.com

## What's here
- `index.html` - Homepage with interactive audio visualizer
- `timeline.html` - Living Timeline (25 synths, all linked to Instagram reels)
- `privacy.html`
- All assets, favicons, OG images

## 1-Click Deploy to Cloudflare Pages

1. Fork this repo or upload these files to a new GitHub repo
2. Go to https://dash.cloudflare.com → Pages → Create project → Connect to Git
3. Select your repo → Framework preset: **None** → Build command: (leave empty) → Deploy
4. Add custom domain `synthnerd.com`

Every `git push` auto-deploys in ~20 seconds.

## Updating daily episodes

Edit `timeline.html` → find `timelineData` array (around line 185):

```javascript
{
  year: 1980,
  name: "TR-808",
  reelUrl: "https://www.instagram.com/reel/YOUR_NEW_ID/",
  // ...
}
```

Commit → Cloudflare auto-updates.

## Local dev
Just open `index.html` in browser. No build step needed.
