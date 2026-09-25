# Degree Speedrun

Pick a degree plan, see which Sophia.org courses clear the most of it, check them off, and watch
the credits and cost drop.

**Live site:** https://vlues.github.io/wgu-speedrun/

## Tabs

- **My Plan**: pick one of 19 degree plans (WGU, UMGC, Embry-Riddle). Shows credits knocked off,
  credits left, what you pay after TA, the best Sophia courses to take next, and a 6-step checklist.
- **Sophia**: every Sophia course, what it clears in your plan, and how many plans it counts in.
- **Compare**: all 19 plans side by side. Tap one to switch to it.
- **Money**: cost after TA, Pell and scholarships; deadlines; a scholarship application tracker.

## Editing

Everything is in [`index.html`](index.html), plain HTML and JavaScript with no build step.
The data lives in clearly labeled lists at the top of the script:

- `PLANS`: degree plans (credits, price, how much JST each can use)
- `SOPHIA`: Sophia courses and what each one clears at each school
- `APPS` and `DEADLINES`: scholarships (a monthly scheduled task keeps these fresh)

Progress is saved in your browser's `localStorage`. Use **Copy backup / Restore backup** at the
bottom to move it to another device.

All numbers are planning estimates. Confirm with each school before paying for anything.
