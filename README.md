# ASCEND

ASCEND is a static, mobile-friendly 100-level calisthenics progression tracker. It starts every athlete at Level 1 and stores all progress in local browser storage. It needs no account, backend, build step, or paid service.

## Use

Open `index.html` in a modern browser, or host the folder from any static web host. The app does not load external images or libraries. Typography uses the device's built-in system fonts.

Choose from three guided exercises in each of the eight pillars, plus a walk/run option. The choices and doses scale with level and prepare you for its harder test stages. Tap any exercise or test standard to read how to perform it. Mark at least four exercises across four different pillars complete to log a qualifying day. The unfinished session stays saved across reloads. No more than one day can count per calendar day. Each level has a three to seven day gate. When unlocked, the rank-up test walks through eight stages, applies the displayed recovery interval between stages, and enforces an overall cap. Stage completion is self-recorded; the tracker does not use sensors to verify form or repetitions. Passing advances one level, records the finish time, and resets the level-specific training-day counter. Local history, personal bests, and test clears remain saved.

Set height in **Progress tools** to show a rough starting walk/run speed range. The app scales a reference speed by the square root of height relative to 170 cm. This is an interface estimate, not a validated personal prescription. The talk test and comfort should determine actual effort; height cannot predict running pace by itself. The [CDC intensity guide](https://www.cdc.gov/physicalactivity/basics/measuring/index.html) describes brisk walking and the talk test. [Running gait research](https://pubmed.ncbi.nlm.nih.gov/28886463/) reports that height relates to stride length, while speed and other factors also affect gait.

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
- `training.js` — graded training menu and exercise instructions
- `.nojekyll` — disable Jekyll processing for static deployment
