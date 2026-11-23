# 🏍️ Commit Ramp Rider

I turned my GitHub contribution graph into a dirt bike track.

Every commit day became a hill. The bigger the day, the bigger the ramp. Zero-commit days are flat road.

Riding my own year was weirdly honest. You can see the deadline sprints. You can see the burnout dips. You can see the exact week I said "I'll just take a short break."

I built Commit Ramp Rider because a contribution graph tells a story, but we only ever glance at it. I wanted to feel it.

It runs in the browser with plain JavaScript. The physics, the dirt bike sound and the graph-to-ramp animation are all custom, with no game engine.

**Live demo: https://awaisdev01.github.io/commit-ramp-rider/**

What would your year look like as a track?

## How it works
- `DAYS` array at the top of `index.html` — put your own `[label, count]` pairs in
- Log-scaled ramp heights so small days still roll and big days actually jump
- Custom spring-free projectile physics with landing dust particles
- WebAudio engine hum (pitch follows speed) + landing thump — no audio files

## License
MIT
