# How to use The U

Two audiences share this file: **families** who want a roster spot, and **maintainers** who update this public hub.

The platform is the live website. There is no account, no dashboard, and no app login.

---

## A. Families — get from first click to The Dojo

Live site: [www.theubasketballprepacademy.com](https://www.theubasketballprepacademy.com/)

### 1. Read the page like a visit

The site is one long page. Use the top nav:

| Nav item | What you will see |
| --- | --- |
| Program | What training covers (skill, IQ, strength, mentorship) |
| A Day at The U | The Monday–Friday clock |
| Academics | Why The U is a training academy, not a school |
| Results / Alumni | Who already placed, and where |
| Founder / Coaches | Coach O and the staff |
| Enrollment | Deposit language and intake windows |
| Contact | Questionnaire, phone, message form |

Two buttons at the top do almost all of the work:

- **Fill out the Questionnaire** — opens the Google Form
- **Book your walkthrough** — opens an email to the academy inbox

### 2. Fill out the Athlete Questionnaire

Open the form: [Athlete Questionnaire](https://docs.google.com/forms/d/e/1FAIpQLScxfI1Vx-FQ5kWW84_TN71jN3_teKjnaNzH5HgntXyayHdfdw/viewform)

It takes about five minutes. You will be asked about the athlete's game, current school situation, and goals. That is how staff decide how to build the path — it is not a public tryout scoreboard.

### 3. Book the walkthrough

After the form, email [theuacademyonline@gmail.com](mailto:theuacademyonline@gmail.com?subject=Walkthrough%20Request%20%E2%80%94%20The%20U%20Prep%20Academy) or call [310.617.3254](tel:+13106173254).

On the visit you should:

- Walk The Dojo at 1219 Los Angeles St., Glendale
- Meet Coach O and staff
- Watch a live session
- Ask every tuition / schedule / school-day question in person

Custom monthly schedules are reviewed during this visit. Dollar amounts are not published on the website or in this repo.

### 4. Confirm the school partner

The U does **not** enroll the student in a school and does **not** issue grades or credits.

You pick:

- an NCAA-approved accredited online school, or
- your own homeschool program

The academy then maps the 12:30–2:30 PM academic block around that school. Parents stay responsible for enrollment, assignments, attendance, and grades.

### 5. Secure the spot upon acceptance

If the family and the academy both say yes, a **non-refundable intake deposit** reserves the roster slot. Training for the 2026–2027 year starts September 8, 2026.

Roster spots stay limited to protect the 2:1 player-to-coach ratio.

### What a weekday looks like (full-time, Glendale)

- 9:00–9:15 AM — Reading & Mindset
- 9:15–9:30 AM — Yoga & Mobility
- 9:30–11:00 AM — The Dojo, team training
- 11:00–11:10 AM — Break
- 11:10 AM–12:00 PM — Individual skill work
- 12:00–12:30 PM — Strength & Conditioning
- 12:30–2:30 PM — Academic block

Part-time training at Jump Beyond Sports (Torrance) runs Tuesday and Thursday, 10:00 AM–12:30 PM.

### Watch before you visit

- Academy POV clip: [x.com/TheUBballPrep](https://x.com/TheUBballPrep/status/2016574805538148822)
- Method on film: [Amen Thompson shooting session](https://www.youtube.com/watch?v=EEU7LLv4NAY)
- Instagram: [@theubasketballprepacademy](https://instagram.com/theubasketballprepacademy)

---

## B. Maintainers — how to update this hub

This repo is a **public citation copy**. The live website is the source of truth.

### Before you change anything

1. Open [www.theubasketballprepacademy.com](https://www.theubasketballprepacademy.com/) and confirm the fact on the page.
2. If the fact is not already public on the site, do not add it here.
3. Never publish tuition dollars, student contact info, medical data, or staff personal emails.

### Update alumni placements

1. Confirm the name and high school are on the live [Alumni section](https://www.theubasketballprepacademy.com/#alumni).
2. Edit `data/placements.csv` **and** `data/placements.json` in the same commit.
3. Bump the JSON `version` field to today's date (`YYYY-MM-DD`).
4. Mirror the same rows in the README alumni table.
5. Follow [docs/DATA.md](DATA.md).

### Update the AI briefing

`llms.txt` in this repo must stay aligned with [the live llms.txt](https://www.theubasketballprepacademy.com/llms.txt).

If the live file changes, copy it here. Do not invent a third version.

### Screenshots in the README

The README hotlinks live images under `https://www.theubasketballprepacademy.com/assets/img/`. Replace the file on the website with the **same filename** and the README image updates on its own. Do not commit binary screenshots to this hub unless the live file is gone.

### What this repo will never contain

- The private website source (`index.html`, CSS, JS, original photography repo)
- Payment forms or dollar amounts
- Student rosters beyond the public alumni table
- Secrets, tokens, or personal inboxes
