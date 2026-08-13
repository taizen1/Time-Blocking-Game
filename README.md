# Golisano Productivity Lab — Time-Blocking Simulation

An interactive, single-file web app that gives incoming students at the Golisano
Institute for Business & Entrepreneurship a hands-on orientation in the full
productivity workflow: inbox triage, brain-dump verification, honest time
estimation, independent study quotas, project chunking, and drag-and-drop
time blocking — with an Orientation Points system that rewards the habits,
not the clicks.

## Run it

Open `index.html` in any modern browser — no build step, no server, no external
dependencies. All CSS and JavaScript are embedded, so the file can be uploaded
as-is to Canvas LMS (Files → embed in a page via iframe) or hosted anywhere.

Progress is saved to the browser's `localStorage`. The **Reset** button starts a
fresh week but keeps earned Orientation Points and badges (achievements are
one-time and can't be farmed by replaying).

## How the simulation works

### Phase 1 — Inbox (Outlook-style mail client)

1. **Sort your inbox.** Nine mock emails from professors (ENT-101, ACC-110,
   COM-105) and internship supervisors arrive unsorted. The student creates
   four topic folders — one per class, one for the internship — and drags each
   email into the folder it belongs in. Misfiled email is accepted but flagged,
   and can't be processed until it's re-filed correctly.
2. **Extract the tasks.** Inside each folder, the student opens every email and
   makes a judgment call: *is someone asking me to do something, or is this
   just context?* Real asks become tasks in the Braindump (major projects
   arrive pre-chunked); FYI emails get archived. Wrong calls get coaching
   feedback and count against the Sharp Eye badge.

### Phase 2 — Weekly Planner

3. **Verify the Braindump.** Extracted tasks start *locked*. Clicking one opens
   a setup panel where the student confirms an estimated completion time (the
   emails say what's expected), a priority level, and sees its hard deadline.
4. **Deconstruct the elephant.** Projects (Market Research Deck, Social Media
   Audit) expand into sequential chunks (Research → Outline → Draft → Polish)
   scheduled individually — with warnings when chunks are placed out of order.
5. **Drag & drop the week.** A Mon–Sun grid with Morning / Afternoon / Evening
   blocks and fixed class sessions locked in. Guardrails give live feedback:
   - **Independent Study Quota meter** — coursework + deep-work hours against
     the 2–3 hours-per-class-hour standard (18–27h), with spawnable Deep Work
     blocks.
   - **Overload / burnout alerts** — red-glow over-capacity blocks, burnout
     days past 9 planned hours, high-priority pile-ups, deadline misses.
6. **Check My Week** — a report card grades the plan across inbox hygiene,
   quota, verification, scheduling coverage, deadlines, capacity, and chunk
   sequencing, with verdicts from 🏆 *Founder-grade week* to 🔥 *This week will
   eat you alive*.

## Orientation Points (⭐ OP)

Fourteen one-time achievements (175 OP total) reward mastery behaviors across
both phases — Inbox Zero, First-Try Filer, Sharp Eye, Elephant Tamer,
Sustainable Scheduler, Spaced Not Crammed, and more. A **Comeback** badge pays
for improving your verdict between reviews, so re-planning is scoring, not
failing. Tiers (Bronze 60 / Silver 110 / Gold 160) track toward the
end-of-orientation award, and the awards panel generates a **completion code**
(a checksum of earned badges) that students submit in Canvas so staff can tally
the cohort.

Anti-gaming by design: achievements never re-award, spamming Check My Week does
nothing, and spawning/deleting study blocks earns nothing on its own.
