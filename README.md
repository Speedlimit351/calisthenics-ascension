# ASCEND

ASCEND is a static, mobile-friendly 100-level calisthenics progression tracker. It starts every athlete at Level 1 and stores all progress in local browser storage. It needs no account, backend, build step, or paid service.

## Use

Open `index.html` in a modern browser, or host the folder from any static web host. The app works offline after its files are available; it does not load external images or libraries. (Typography uses the device's built-in system fonts.)

Log no more than one qualifying training day per calendar day. Each level has a three to seven day gate. When unlocked, the rank-up test walks through eight stages, applies the displayed recovery interval between stages, and enforces an overall cap. Stage completion is self-recorded; the tracker does not use sensors to verify form or repetitions. Passing advances one level, records the finish time, and resets the level-specific training-day counter. Local history, personal bests, and test clears remain saved.

Use **Progress tools** to download a JSON backup or restore one. Clearing browser site data removes progress unless a backup exists.

## The 10 ranks

| Levels | Rank | Focus |
|---|---|---|
| 1–10 | Foundation | Movement basics and foundational hangs |
| 11–20 | Initiate | Pull-ups, pistols, tuck holds, first freestanding balance |
| 21–30 | Athlete | Weighted strength, handstand control, lever progressions |
| 31–40 | Intermediate | Muscle-up entry, stronger levers, handstand push-ups |
| 41–50 | Advanced | Freestanding pressing, harder lever variations |
| 51–60 | Expert | Full front lever, straddle planche, V-sit |
| 61–70 | Elite | One-arm pulling, planche and press-handstand milestones |
| 71–80 | Master | One-arm handstand and 90-degree pressing progressions |
| 81–90 | Grandmaster | High-end one-arm, planche and press skills |
| 91–100 | Superhuman | Deliberately beyond typical human performance |

Every level spans push, pull, legs, core/compression, balance/inversion, straight-arm/rings, mobility/control, and grip/explosiveness. Level 1–10 follow the detailed standards preserved from the original progression. The referenced conversation's cached copy ended during Level 80, so later-level standards are generated as a smoothly escalating continuation; Level 100 is explicitly a superhuman target. Training standards and timed circuits are editable in `app.js`.

## Publish with GitHub Pages

Create a **public** repository, add these files to its default branch, then in repository **Settings → Pages**, choose **Deploy from a branch**, select the default branch and `/ (root)`, and save. GitHub Pages is suitable for this static site. The repository/account must have Pages access enabled. Progress stays in each visitor's own browser and is not synced between devices.

## Files

- `index.html` — page structure and dialogs
- `style.css` — responsive dark visual system
- `app.js` — progression standards, local storage, history, achievements, timers
- `.nojekyll` — disable Jekyll processing for static deployment
