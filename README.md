# Aryan Sajiv

Computer Science student at the University of Manchester building full-stack web applications, with a focus on database design, security and applied AI.

[Email](mailto:aryansajiv2@gmail.com) · [Projects](#selected-projects)

## Overview

I build applications end to end, from schema design and access control in PostgreSQL to type-safe React front ends, automated tests and deployment. My projects put the rules that matter in the database, measure performance before and after changes, and test at the database, unit and browser levels.

## Selected projects

### [Tip of the Tongue](https://github.com/aryansajiv19/Tip-of-the-Tongue)

<a href="https://github.com/aryansajiv19/Tip-of-the-Tongue"><img src="https://raw.githubusercontent.com/aryansajiv19/Tip-of-the-Tongue/main/docs/assets/demo.gif" alt="Tip of the Tongue overlay offering the word a speaker stalled on" width="640"></a>

A live word-finding companion for people who lose words mid-conversation: it listens, notices when the speaker stalls, and offers the likely word in a small overlay, staying silent otherwise. Hiya Voice AI Challenge entry, Real-time Assistance track.

- A speculative guess starts about 0.3 s into a pause, so the word appears about 1.5 s after the last spoken word; a confidence gate keeps it quiet on fluent speech (0–1 pop-ups in 165 fluent lines).
- A prompt pass raised accuracy from 85–90% to 93–96% across 20 scripted conversations, and 94% on a held-out set it was never tuned on.
- Speaker diarisation decides whose pauses count, the pause threshold adapts to each speaker's pace, and the pipeline recovers from network drops, sleep and microphone changes.

TypeScript, Node.js (Fastify, WebSockets), React, Electron, Deepgram Nova-3, Claude Haiku, Vitest, Playwright

### [SkillVerse](https://github.com/aryansajiv19/SkillVerse)

<a href="https://skillverse-sable.vercel.app"><img src="https://raw.githubusercontent.com/aryansajiv19/SkillVerse/main/docs/media/constellations.jpg" alt="SkillVerse skill graph with completed learning paths" width="640"></a>

A learning platform that models a curriculum as a skill graph, builds a personalised path to any skill, and grades knowledge checks inside PostgreSQL.

- Leaderboard rank was recomputed per row, so a public filter could trigger quadratic work; a single window function reduced it from 5.4 s to 3.4 ms at 10,000 players.
- The answer key lives in a schema the API cannot read, and CI fails the build if an answer appears in the client bundle.
- 63 database, 220 unit and 19 browser tests, including WCAG 2.1 AA scans.

React, TypeScript, Supabase (PostgreSQL, RLS, Realtime), Playwright, pgTAP · [Live demo](https://skillverse-sable.vercel.app)

### [Planind](https://github.com/aryansajiv19/plan-ind)

<a href="https://plan-ind.vercel.app"><img src="https://raw.githubusercontent.com/aryansajiv19/plan-ind/main/docs/media/flow.gif" alt="Planind group voting through elimination rounds" width="640"></a>

A real-time group planning app: the host sets constraints, the app shortlists venues, and the group votes through elimination rounds.

- Ballots are cast only through database functions, so concurrent duplicate votes resolve to one row, verified by race-condition tests.
- A trigram index cut unmatched venue searches from 2.26 ms to 0.07 ms; 200 simultaneous voters completed in under 250 ms.
- URL imports are protected against SSRF, including DNS rebinding.

Next.js, React 19, TypeScript, Supabase, OpenAI · [Live demo](https://plan-ind.vercel.app)

### [ASCEND](https://github.com/aryansajiv19/ASCEND)

A training app that scores per-muscle recovery from recent workouts and provides an AI coach grounded in the user's own history.

- Deterministic recovery model over seven days of training volume and elapsed time.
- Natural-language workout logging, with unparseable model output rejected rather than stored.
- Live challenge leaderboards over WebSockets, pushed only to the rooms a participant has joined.

Node.js, Express, PostgreSQL, React, Claude, Docker

### Earlier work

- [MU0 Memory Game](https://github.com/aryansajiv19/MU0-memory-game): a game in MU0 assembly using memory-mapped keypad, display and buzzer I/O on an eight-instruction processor.
- [Automobile Management System](https://github.com/aryansajiv19/Automobile-Management-System): a command-line dealership records system using pandas and MySQL.

## Stack

**Languages:** TypeScript, JavaScript, Python, SQL  
**Frontend:** React, Next.js, Tailwind CSS, Electron  
**Backend:** Node.js, Express, Supabase, PostgreSQL (RLS, PL/pgSQL, triggers, indexing)  
**AI:** OpenAI, Claude and Gemini APIs, structured outputs, Deepgram speech-to-text  
**Testing:** Vitest, Playwright, pgTAP  
**Infrastructure:** GitHub Actions, Docker, Vercel

## Contact

Open to software engineering internships and graduate roles: [aryansajiv2@gmail.com](mailto:aryansajiv2@gmail.com)
