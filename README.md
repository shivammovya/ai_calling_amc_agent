# ai_calling_amc_agent

Call analytics dashboard for **AMC Sahayak**, the AI voice agent that takes citizen complaints
(garbage, stray animals, potholes, fallen trees, waterlogging, ...) for the Ahmedabad Municipal
Corporation.

- `data/Recordings/rec_N.mp3` and `data/Transcript/tran_N.txt`: raw call recordings and transcripts
- `data/calls.json`: one structured record per call (caller, area, location, complaints + category, summary)
- `dashboard/calls_data.js`: the same records loaded by the static dashboard. Keep it in sync with `data/calls.json`
- `dashboard/`: static site (Overview, Calls, Follow-up, Analytics)

Run locally with `python -m http.server` from the repo root and open http://localhost:8000/dashboard/
