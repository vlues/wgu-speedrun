# Degree Speedrun Tracker

A single-page site that lays out a "speedrun" route through WGU's **BS Cloud and Network Engineering**
(the degree that replaced BS Cloud Computing) — cheapest courses first via Sophia.org, then WGU —
with checkboxes to track what you've completed.

**Live site:** https://vlues.github.io/wgu-speedrun/

## How it works

- Everything is in one file: [`index.html`](index.html). No frameworks, no build step.
- The route/course data is a plain JavaScript array near the top of the `<script>` tag
  (`BUILT_IN_PLANS`) — edit it there to change courses, CUs, or tips.
- Progress, custom plans, and your selected plan are saved in your browser's
  `localStorage`, so the site remembers your checkmarks between visits.
  (Per-browser/per-device — clearing site data resets it.)
- **＋ New plan** lets you track a different school/degree entirely: name it, add phases
  and courses right on the page. Custom plans are also saved locally.

## Editing / deploying

Edit `index.html`, then:

```
git add -A && git commit -m "update" && git push
```

GitHub Pages redeploys automatically from the `main` branch.

> Note: course mappings and WGU program details change often — always confirm against
> WGU's official transfer pathways and an enrollment counselor before spending money.
