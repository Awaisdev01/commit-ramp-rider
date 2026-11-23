# 🏍️ Commit Ramp Rider

I turned my GitHub contribution graph into a dirt bike track.

Every commit day became a hill. The bigger the day, the bigger the ramp. Zero-commit days are flat road.

Riding my own year was weirdly honest. You can see the deadline sprints. You can see the burnout dips. You can see the exact week I said "I'll just take a short break."

I built Commit Ramp Rider because a contribution graph tells a story, but we only ever glance at it. I wanted to feel it.

It runs in the browser with plain JavaScript. The physics, the dirt bike sound and the graph-to-ramp animation are all custom, with no game engine.

**Live demo: https://awaisdev01.github.io/commit-ramp-rider/**

What would your year look like as a track?

## Gameplay

- **Real slope physics** — gravity pulls you down slopes and slows you on climbs
- **Air control** — rotate with ↑/↓ and land flat, or crash (checkpoint retry)
- **Commit coins** — every ramp spawns coins scaled to that day's commits; grab them mid-air
- **Score** — air time, coins, and clean landings; combos pop as you ride
- **Space = boost** — more speed, higher launches (mobile: hold the screen)
- Crash into a wall with too little speed and you're walking home

## How it works
- `DAYS` array at the top of `index.html` — put your own `[label, count]` pairs in
- Log-scaled ramp heights so small days still roll and big days actually jump
- Heightfield terrain with O(1) sampling, slope-projected gravity, landing-angle checks
- WebAudio engine hum (pitch follows speed), landing thumps, coin dings — no audio files

## License
MIT
