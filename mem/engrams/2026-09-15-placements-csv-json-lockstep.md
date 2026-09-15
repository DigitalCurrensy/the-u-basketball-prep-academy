---
slug: placements-csv-json-lockstep
created: 2026-09-15
weight: 0.94
tags: [data, schema]
source: incident
---
# What happened
Alumni data is seven public high-school placements. CSV has per-row `source`. JSON does not. Version is 2026-08-05. Three notes are empty on purpose.

# Why it matters
This is not a SIS. Live site #alumni is source of truth. CSV and JSON must describe the same athletes. Edit both files and the README table in the same commit. Bump JSON `version` to the ship date. Do not invent accolades or extra fields (no staff.json, no student roster).

# Trigger
Any change to data/placements.csv or data/placements.json.
