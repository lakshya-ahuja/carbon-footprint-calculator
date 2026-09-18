Carbon Footprint Tracker - Hackathon Rules (Concise)
1. Core MVP & Product Goal
Build a responsive app to log activities, calculate CO₂, track weekly targets, view history, and receive supportive nudges.

Activities: Car (km), Bus (km), Flight (km), Electricity (kWh), Veg Meal (meal), Non-Veg Meal (meal).
Week Definition: Always Monday 00:00 → Sunday 23:59.
2. CO₂ Calculations (Strict Fixed Factors)
Backend must perform the final calculation (CO₂ = quantity × factor). Store factors centrally.

Car: 0.20 kg CO₂ / km
Bus: 0.08 kg CO₂ / km
Flight: 0.25 kg CO₂ / km
Electricity: 0.80 kg CO₂ / kWh
Veg meal: 0.50 kg CO₂ / meal
Non-veg meal: 2.00 kg CO₂ / meal
3. Dashboard
Show: Weekly total, weekly target, target progress (%), and amount remaining/exceeded.
Category Breakdown: Transportation (Car/Bus/Flight), Electricity, Food (Veg/Non-veg).
Target Exceeded: Clearly show the exceeded amount. Never hide it.
4. Input Validation & Absurd Inputs
Validate: > 0, numeric, valid activity type, no empty fields.
Absurd Input: Warn user on extremely high values (e.g., 50,000 km) and ask for confirmation. Do not block or delete without explanation.
Security: Never trust frontend data. Backend must re-validate everything.
5. Nudges (Supportive & Non-Judgmental)
Target Exceeded: Show a clear, supportive warning stating the current total, target, amount over, and an actionable suggestion.
Rule: Do not shame, punish, or block functionality.
6. History & Data Model
History: Sort newest first. Support filtering by category/type and date/week.
Immutability: Store calculated CO₂ value at creation time (do not recalculate historical data if factors change later).
Core Entities: Users, Activities, Targets, Notifications/Nudges.
7. UX & Error Handling
UI: Mobile-first, clear visual hierarchy, large numbers for totals, accessible.
States: Handle Loading, Error, Empty (e.g., no history), First-Time (set target), and Edge states gracefully.
Feedback: Never expose raw server errors to users.
8. Build Priorities
Core: Setup, Activity logging, CO₂ math, Dashboard total.
Required: Category breakdown, Weekly target/progress, History & filters.
Logic: Nudges, Absurd input warnings, Strict Mon-Sun logic.
Polish: Responsive UI, Charts, Loading/Error states, Accessibility.