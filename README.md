# Hi, I'm Aryan 👋

I'm a penultimate-year **Computer Science** student at the **University of Manchester**. I build full-stack products end to end, from the database rules up to the last bit of UI polish, and I'm most interested in anything where AI and software meet a real problem people have.

What I like to show in my projects isn't only that they work, but *why* they hold up: the security model, the tests, and numbers I've actually measured.

## 🚀 Selected projects

<table>
<tr>
<td width="46%"><a href="https://skillverse-sable.vercel.app"><img src="https://raw.githubusercontent.com/aryansajiv19/SkillVerse/main/docs/media/path.jpg" alt="SkillVerse: clicking a star lights up the learning path to it"></a></td>
<td>

### [SkillVerse](https://github.com/aryansajiv19/SkillVerse)
**A personalised learning path, laid out as a galaxy.** Click any skill and the stars you need light up in order, each with a lesson, free resources, practice and a knowledge check.

- Quizzes are graded inside Postgres, and CI proves the answers never ship to the browser
- Replaced a quadratic leaderboard query: **5.4 s → 3.4 ms** at 10,000 players
- 63 database tests, 215 unit tests, 19 end-to-end tests with accessibility scans

React · TypeScript · Supabase (Postgres, RLS, Realtime) · Three.js · Playwright
[**Live demo**](https://skillverse-sable.vercel.app) · [Code](https://github.com/aryansajiv19/SkillVerse)

</td>
</tr>
<tr>
<td width="46%"><a href="https://plan-ind.vercel.app"><img src="https://raw.githubusercontent.com/aryansajiv19/plan-ind/main/docs/media/flow.gif" alt="plan-ind: a group voting through three rounds to a winner"></a></td>
<td>

### [plan-ind](https://github.com/aryansajiv19/plan-ind)
**Group plans in Dubai, decided in three rounds instead of three hundred messages.** Friends vote on places live, and the plan carries on into RSVPs, carpools and calendar invites.

- Every vote goes through a database function, so nobody can fake or double a vote
- Search index took a failed search at 5,000 places from **2.26 ms to 0.07 ms**
- 200 people voting at the same moment finished in **under 250 ms**; 213 Playwright tests

Next.js · React 19 · Supabase · OpenAI
[**Live demo**](https://plan-ind.vercel.app) · [Code](https://github.com/aryansajiv19/plan-ind)

</td>
</tr>
<tr>
<td width="46%"><a href="https://github.com/aryansajiv19/ASCEND"><img src="https://raw.githubusercontent.com/aryansajiv19/ASCEND/main/docs/dashboard.png" alt="ASCEND dashboard with per-muscle recovery scores"></a></td>
<td>

### [ASCEND](https://github.com/aryansajiv19/ASCEND)
**AI fitness coaching that knows how recovered each muscle is.** Log a workout by just describing it, and a coach answers with your full training history in view.

- Per-muscle recovery scores computed from training volume and recency
- An LLM coach with access to your workouts, plus voice logs parsed into structured data
- Live challenges and leaderboards over WebSockets, with full-text workout search

Node.js · Express · PostgreSQL + pgvector · React · Claude · Docker
[Code](https://github.com/aryansajiv19/ASCEND)

</td>
</tr>
</table>

## 🛠️ What I work with

- **Full-stack web:** React, Next.js and TypeScript on the front; Node.js and Express behind them.
- **Databases:** PostgreSQL in depth: row-level security, triggers, full-text search, pgvector, and profiling queries with `EXPLAIN ANALYZE`. Supabase for auth, Realtime and edge functions.
- **AI features:** building products on LLMs (Claude, OpenAI, Gemini), such as tutors, coaches, and turning plain English into structured data.
- **Quality and delivery:** Vitest, Playwright, pgTAP and axe for accessibility; GitHub Actions, Docker and Vercel.
- **Languages:** TypeScript, JavaScript, Python, SQL.

## 📫 Get in touch

I'm always happy to talk about AI, software, or opportunities to work on either.

✉️ [aryansajiv2@gmail.com](mailto:aryansajiv2@gmail.com)
