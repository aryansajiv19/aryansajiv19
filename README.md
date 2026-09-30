# Aryan Sajiv

Computer Science undergraduate (penultimate year) at the University of Manchester, focused on full-stack systems, database engineering and applied AI.

[Email](mailto:aryansajiv2@gmail.com) · [GitHub](https://github.com/aryansajiv19)

## Summary

I design and ship production web applications end to end: data modelling and access control in PostgreSQL, APIs and server logic, type-safe React front ends, automated testing and continuous deployment. My projects emphasise measurable performance, explicit security models and test coverage at the database, unit and browser levels.

## Selected projects

<table>
<tr>
<td width="44%"><a href="https://skillverse-sable.vercel.app"><img src="https://raw.githubusercontent.com/aryansajiv19/SkillVerse/main/docs/media/constellations.jpg" alt="SkillVerse skill graph with completed learning paths"></a></td>
<td>

### [SkillVerse](https://github.com/aryansajiv19/SkillVerse)
Personalised learning paths on an interactive skill graph, with server-graded knowledge checks.

- Quiz grading and mastery in atomic PostgreSQL functions; the answer key is held in an unexposed schema and CI verifies it never reaches the client bundle
- Replaced a quadratic leaderboard query with a window function: **5.4 s → 3.4 ms** at 10,000 players; **>120 s → 17.6 ms** at 50,000
- Row-level security with least-privilege and column-level grants, enforced by schema-wide pgTAP invariants in CI
- 63 database, 220 unit and 19 end-to-end tests, including WCAG 2.1 AA scans

React · TypeScript · Supabase (PostgreSQL, RLS, Realtime) · Playwright · pgTAP
[Live demo](https://skillverse-sable.vercel.app) · [Source](https://github.com/aryansajiv19/SkillVerse)

</td>
</tr>
<tr>
<td width="44%"><a href="https://plan-ind.vercel.app"><img src="https://raw.githubusercontent.com/aryansajiv19/plan-ind/main/docs/media/flow.gif" alt="Planind group voting through elimination rounds"></a></td>
<td>

### [Planind](https://github.com/aryansajiv19/plan-ind)
Real-time group decision-making: shortlist venues, vote in elimination rounds, then coordinate the outing.

- Ballots cast only through database functions; concurrent duplicate votes resolve to a single row, verified by race-condition tests
- Trigram GIN index reduced unmatched venue search from **2.26 ms to 0.07 ms** (30×); 200 simultaneous voters completed in under 250 ms
- SSRF-hardened URL import with DNS-rebinding protection; LLM search constrained by JSON Schema output and hermetic guardrail tests
- 380+ unit, 170+ database and cross-browser Playwright tests

Next.js · React 19 · TypeScript · Supabase · OpenAI
[Live demo](https://plan-ind.vercel.app) · [Source](https://github.com/aryansajiv19/plan-ind)

</td>
</tr>
<tr>
<td width="44%"><a href="https://github.com/aryansajiv19/ASCEND"><img src="https://raw.githubusercontent.com/aryansajiv19/ASCEND/main/docs/dashboard.png" alt="ASCEND dashboard with per-muscle recovery scores"></a></td>
<td>

### [ASCEND](https://github.com/aryansajiv19/ASCEND)
AI fitness coaching with per-muscle recovery scoring, natural-language logging and live challenges.

- Deterministic recovery model over seven days of training volume and elapsed time
- Streaming LLM coach grounded in the user's workout history and recovery state
- Natural-language logging parsed into validated structured records
- Real-time challenge leaderboards over WebSockets; containerised with Docker

Node.js · Express · PostgreSQL · React · Claude · Docker
[Source](https://github.com/aryansajiv19/ASCEND)

</td>
</tr>
</table>

### Other work

| Project | Description |
|---|---|
| [MU0 Memory Game](https://github.com/aryansajiv19/MU0-memory-game) | Interactive game in MU0 assembly using memory-mapped keypad, display, LED and buzzer I/O on an eight-instruction processor |
| [Automobile Management System](https://github.com/aryansajiv19/Automobile-Management-System) | Command-line dealership records system with pandas, MySQL and matplotlib |

## Technical skills

| Area | Tools |
|---|---|
| Languages | TypeScript, JavaScript, Python, SQL |
| Front end | React, Next.js, Tailwind CSS, Vite |
| Back end | Node.js, Express, Supabase (Auth, Realtime, Edge Functions), REST, WebSockets |
| Databases | PostgreSQL: row-level security, PL/pgSQL, triggers, indexing, full-text and trigram search, pgvector, query analysis with `EXPLAIN ANALYZE` |
| AI | OpenAI, Anthropic Claude and Gemini APIs; structured outputs, streaming, evaluation |
| Testing | Vitest, Playwright, pgTAP, axe accessibility testing, load testing |
| Delivery | GitHub Actions, Docker, Vercel |

## Contact

Open to software engineering internships and graduate opportunities. Reach me at [aryansajiv2@gmail.com](mailto:aryansajiv2@gmail.com).
