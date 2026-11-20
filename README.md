# RBC Pulse
**Career development for RBC early talent: find your path, close your gaps, and stay.**

> Built for the RBC WTAP Hackathon.

RBC Pulse is a web app with three views: students, mentors and program coordinators. Students use it to discover internal career paths, see exactly which skills they're missing and follow a roadmap to get there. Program coordinators use the same data to spot students at risk of leaving and to find gaps in RBC's programs before they turn into problems.

---

## Our Idea

Students often leave when they **can't see a future** at the company. RBC Pulse makes that future visible:

```
Survey  →  Pick a role  →  See your skill gaps  →  Follow a roadmap  →  Get support
                                                          │
                              Coordinators see who's stalling and what's missing
```

When a student stops making progress toward the goal they chose, that's an early warning sign. RBC Pulse turns career development into a **retention signal**.

---

## Features

### For Students

| Feature | What it does |
|---|---|
| **Internal Career Discovery** (MVP) | A multiple-choice survey on interests (e.g., *Cybersecurity → SOC Analyst*). Students enter their current role and team, then rate their skills. AI suggests 2–3 matching RBC roles; they pick one or type their own. |
| **Skill Gap Plan** (MVP) | For the chosen role: what it does, which RBC teams have it and the skills it needs. Students rate their skills or upload a resume, and RBC Pulse shows what they have, what's missing (e.g., *"Your biggest gap is SQL: 2 → 4"*) and a **Recommended next steps** dropdown (workshops, courses, repos). |
| **Roadmap & Progress Tracker** (MVP) | A step-by-step plan: an internal course, a small project on their team, a coffee chat with someone in the role, a rotation (Quest / Boost). Students check off steps and watch the progress bar grow. |
| **"How They Got There" Stories** (MVP) | Anonymized career paths from current employees, shown as a simple timeline. |
| **Job Posting Matcher** | A student pastes an internal job posting. RBC Pulse pulls out the required skills, compares them to the student's profile and shows the match: *"You match 4/7 skills."* Missing skills link to next steps. |
| **Pulse Feedback** | After an onboarding session, training or mentor meeting, a one-tap prompt asks *"How was this?"* (positive, neutral or negative) with an optional comment. A feedback button is always available, so students can share how they feel at any time. |
| **Bi-weekly Check-in** | *"How's it going?"* and *"Do you see a future at RBC?"*, each rated 1–5. |
| **Learning Plan Saver** | Paste a link to any course, repo or article to add it to the learning plan for a target role. |
| **"You Said, We Did" Feed** | In-app updates that show how feedback led to change: *"You said onboarding was confusing → we added a checklist."* |

### For Mentors & Managers

| Feature | What it does |
|---|---|
| **Mentee View** (MVP) | See a student's target role and progress, plus suggested conversation starters for 1:1s. |
| **Endorse a Skill** | A mentor confirms the student showed a skill on the job. This carries more weight than self-reporting. |

### For Program Coordinators (web dashboard)

| Feature | What it does |
|---|---|
| **Talent Demand Map** (MVP) | Which roles students want vs. where RBC actually has openings, so mismatches show up early. |
| **Stalled-Path Flags** (MVP) | Students with no progress for 3+ weeks, a falling "future at RBC" score, or no clear path to their chosen role are flagged as **retention risks**. |
| **Program Gap Insights** | e.g., *"35 students need SQL for their target roles, but there's no internal SQL training"* → a systemic fix. |
| **Cohort History** | Keeps historical data on which paths past students took and who got return offers, so future recommendations improve. |

Items marked (MVP) are in scope for the 1-day build.

---

## Privacy by Design

- **No email and no full name.** Each student gets a random anonymous ID and returns with an anonymous access code instead of personal details.
- The dashboard shows aggregated insights; retention flags go to program coordinators, not to a student's manager.

---

## Fits With What RBC Already Has

RBC Pulse doesn't replace existing programs. It **plugs into them**:

- **Quest** and **Boost** (new-grad rotational program) appear as roadmap steps, e.g., *"Apply to the Boost security rotation."*
- The demand map shows program leads which rotations and tracks students actually want.

---

## Tech Stack

| Part | Tech |
|---|---|
| Web app | *Framework TBD by the web team* (student, mentor and coordinator views) |
| Backend & database | *TBD* (stores anonymous profiles, feedback and historical cohort data) |
| AI | One LLM call: resume + role description → personalized gap plan; interests → role suggestions |
| Data | Role catalog JSON (roles, teams, skills, resources). HR can swap it for real job-architecture data. |

---

## Getting Started

```bash
git clone https://github.com/samaasrr/wtap-hackathon.git
cd wtap-hackathon
```

*(Install and run steps will be added once the web app code is in the repo.)*

---

## Demo Flow


**The loop:** set a goal → see the path → make progress → get support → spot risk → fix the system → follow up.

---

## Team

*Add names and roles here.*
