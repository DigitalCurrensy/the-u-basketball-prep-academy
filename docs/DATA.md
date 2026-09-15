# Alumni placements data

This folder holds the only dataset in the public hub: **high-school placements already published on the academy website**.

Source of truth: [www.theubasketballprepacademy.com/#alumni](https://www.theubasketballprepacademy.com/#alumni)

Current snapshot: **7 athletes**, version **2026-08-05**.

---

## Files

| File | Form | Use |
| --- | --- | --- |
| [`data/placements.csv`](../data/placements.csv) | Spreadsheet | Humans, Sheets, quick diffs |
| [`data/placements.json`](../data/placements.json) | JSON envelope + array | Sites, scripts, citations |

Both files must describe the same seven people. If they drift, the website Alumni section wins.

---

## CSV columns

| Column | Type | Required | Notes |
| --- | --- | --- | --- |
| `athlete` | string | yes | Public name as it appears on the site. Unique inside one snapshot. |
| `high_school` | string | yes | School name only — no address. |
| `note` | string | no | Public accolade already on the site. Empty string is allowed. |
| `source` | URL | yes in CSV | Currently the Alumni section URL for every row. |

Example row:

```csv
Will Conroy Jr.,Village Christian,Top Freshman in the Country,https://www.theubasketballprepacademy.com/#alumni
```

---

## JSON envelope

```json
{
  "dataset": "The U Basketball Prep Academy — Alumni Placements",
  "version": "2026-08-05",
  "publisher": {
    "name": "The U Basketball Prep Academy",
    "url": "https://www.theubasketballprepacademy.com/"
  },
  "license": "All rights reserved — cite with attribution to The U Basketball Prep Academy",
  "source": "https://www.theubasketballprepacademy.com/#alumni",
  "placements": [
    {
      "athlete": "Will Conroy Jr.",
      "high_school": "Village Christian",
      "note": "Top Freshman in the Country"
    }
  ]
}
```

JSON rows do **not** repeat `source` per athlete. The envelope `source` covers the set.

Known shape difference: CSV has a per-row `source` column; JSON does not. That is intentional. Do not invent extra JSON fields to "match" the CSV unless you are adding a real new public attribute.

---

## Current rows

| Athlete | High school | Note |
| --- | --- | --- |
| Will Conroy Jr. | Village Christian | Top Freshman in the Country |
| Luke Sowby | Salesian | All-CIF as a Freshman |
| Alfred "Deebo" Parker | Taft High | Starting Varsity |
| Dominik Karapetian | Brentwood | Playing Varsity |
| Noah Austin | Fairfax | *(empty)* |
| Bryce Bible | St. John Bosco | *(empty)* |
| Jeremy Robinson | Servite | *(empty)* |

Empty notes stay empty. Do not fill them from memory.

---

## How to add or change a row

1. Confirm the athlete is already named on the live Alumni section.
2. Edit CSV and JSON in the **same commit**.
3. Keep `Alfred "Deebo" Parker` quoted exactly that way.
4. Set JSON `version` to the ship date (`YYYY-MM-DD`).
5. Update the alumni table in `README.md` so the three copies agree.
6. Do not add a person who is only on a private roster.

---

## Not in this dataset

Do not add any of the following, here or in a new file:

- Emails, phones, parent contacts, home addresses
- Date of birth, grade, height, weight, GPA
- Medical or emergency information
- Tuition, deposits as dollar amounts, payment plans
- Staff personal inboxes
- Full student rosters
- Photos of minors beyond what the public website already hosts

This is not a student-information system. It is a public citation table.

---

## License

All rights reserved. Cite with attribution to The U Basketball Prep Academy. No redistribution or reuse permission is granted.
