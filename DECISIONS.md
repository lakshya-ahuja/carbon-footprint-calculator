# Decisions

## DP1 — The nudge
**Decision:** Warn, don't block. Crossing the weekly target shows a red banner (kg over + one targeted tip) — nothing is rejected.
**Why:** The app's job is awareness, not enforcement; blocking would stop it reflecting real behavior right when that matters most.

## DP2 — Absurd input
**Decision:** Allow, but warn inline. Each activity type has a soft threshold (e.g. 1,000 km, 200 kWh, 10 meals) that triggers a caution, not a rejection.
**Why:** Most absurd numbers are typos, not lies — a soft check catches mistakes without blocking legitimate edge cases like a long-haul flight.

## DP3 — The week
**Decision:** Monday–Sunday, with live progress updated after every log or reset.
**Why:** Monday-start matches how people plan their week, and live progress lets users course-correct mid-week instead of Sunday night.
