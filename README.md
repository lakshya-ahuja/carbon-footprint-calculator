**Hackathon ID:** AZIS-484ZEN
**Team Emails:** lakshyaahuja00@gmail.com · sangwanvarsha2007@gmail.com

---

Carbon Footprint Tracker

*Smaller choices. Bigger impact.*

A simple web app that turns your daily activities into a weekly carbon budget. Log a car ride, a meal, or an electricity reading, and it's converted to kg CO₂ using fixed emission factors — no estimating required.

**Live demo:** https://lakshya-ahuja.github.io/carbon-footprint-calculator/hackathon/

## Features

- Log activities (car, bus, flight, electricity, meals) with live CO₂ calculation
- Running weekly ledger of all logged entries, newest first
- Weekly CO₂ target with progress bar and over/under-budget nudges
- Data persists locally in the browser between visits

## CO₂ Calculation

`CO₂ produced = quantity × emission factor`

| Activity | Factor |
|---|---|
| Car | 0.20 kg / km |
| Bus | 0.08 kg / km |
| Flight | 0.25 kg / km |
| Electricity | 0.80 kg / kWh |
| Vegetarian meal | 0.50 kg / meal |
| Non-vegetarian meal | 2.00 kg / meal |

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript (React/Next.js + Tailwind planned for next iteration)
- **Backend (planned):** Node.js / Express or FastAPI
- **Database (planned):** PostgreSQL / MongoDB
- **Hosting:** GitHub Pages
