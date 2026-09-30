# Aryan Sajiv

Computer Science student at the University of Manchester, in my penultimate year.

I like building things people actually want to open: a learning app that looks like a night sky, a planner that ends the "so where are we going?" group chat, a training coach that knows which muscles are still sore. I'm happiest when an idea turns into something friends can use, and I take projects the whole way, from database design and security to tests, deployment and the small details that make them fun.

Lately I've been most interested in where AI makes software more useful, not just more impressive.

## Projects

<table>
<tr>
<td width="46%"><a href="https://skillverse-sable.vercel.app"><img src="https://raw.githubusercontent.com/aryansajiv19/SkillVerse/main/docs/media/constellations.jpg" alt="SkillVerse: finished learning paths formed as gold constellations on the galaxy map"></a></td>
<td>

### [SkillVerse](https://github.com/aryansajiv19/SkillVerse)
A learning app where every path is a constellation. Pick a skill and the stars you need light up in order, each with a lesson, free resources and a knowledge check. It started at a hackathon; I rebuilt it into a full-stack app.

- Quizzes are graded inside Postgres, and CI proves the answers never ship to the browser
- Replaced a quadratic leaderboard query: **5.4 s → 3.4 ms** at 10,000 players
- Tested at three layers: database (pgTAP), unit (Vitest) and end-to-end with accessibility scans (Playwright + axe)

React · TypeScript · Supabase (Postgres, RLS, Realtime) · Three.js · Playwright
[Live demo](https://skillverse-sable.vercel.app) · [Code](https://github.com/aryansajiv19/SkillVerse)

</td>
</tr>
<tr>
<td width="46%"><a href="https://plan-ind.vercel.app"><img src="https://raw.githubusercontent.com/aryansajiv19/plan-ind/main/docs/media/flow.gif" alt="plan-ind: a group voting through three rounds to a winner"></a></td>
<td>

### [plan-ind](https://github.com/aryansajiv19/plan-ind)
Group plans in Dubai, decided in three rounds instead of three hundred messages. Friends vote on places live, and the plan carries on into RSVPs, carpools and calendar invites.

- Every vote goes through a database function, so nobody can fake or double a vote
- Search index took a failed search at 5,000 places from **2.26 ms to 0.07 ms**
- 200 people voting at the same moment finished in **under 250 ms**; 213 Playwright tests

Next.js · React 19 · Supabase · OpenAI
[Live demo](https://plan-ind.vercel.app) · [Code](https://github.com/aryansajiv19/plan-ind)

</td>
</tr>
<tr>
<td width="46%"><a href="https://github.com/aryansajiv19/ASCEND"><img src="https://raw.githubusercontent.com/aryansajiv19/ASCEND/main/docs/dashboard.png" alt="ASCEND dashboard with per-muscle recovery scores"></a></td>
<td>

### [ASCEND](https://github.com/aryansajiv19/ASCEND)
AI fitness coaching that knows how recovered each muscle is. Describe a workout in plain words and it gets logged; the coach answers with your full training history in view.

- Per-muscle recovery scores computed from training volume and recency
- An LLM coach with access to your workouts, plus voice logs parsed into structured data
- Live challenges and leaderboards over WebSockets, with full-text workout search

Node.js · Express · PostgreSQL + pgvector · React · Claude · Docker
[Code](https://github.com/aryansajiv19/ASCEND)

</td>
</tr>
</table>

## What I work with

- **Web:** TypeScript, React and Next.js, with Node.js and Express on the server
- **Data:** PostgreSQL (row-level security, triggers, full-text search, pgvector, query tuning with `EXPLAIN ANALYZE`) and Supabase
- **AI:** products built on Claude, OpenAI and Gemini, from tutors and coaches to turning plain English into structured data
- **Quality and shipping:** Vitest, Playwright, pgTAP, axe, GitHub Actions, Docker, Vercel
- **Languages:** TypeScript, JavaScript, Python, SQL

## Contact

Always up for a chat about AI, side projects, hackathons or roles where I can build things like these.

[aryansajiv2@gmail.com](mailto:aryansajiv2@gmail.com)
