# Golisano Productivity Lab — Time-Blocking Simulation

An interactive, single-file web app that gives incoming students at the Golisano
Institute for Business & Entrepreneurship a hands-on orientation in realistic
weekly planning: brain-dump verification, honest time estimation, independent
study quotas, project chunking, and drag-and-drop time blocking.

## Run it

Open `index.html` in any modern browser — no build step, no server, no external
dependencies. All CSS and JavaScript are embedded, so the file can be uploaded
as-is to Canvas LMS (Files → embed in a page via iframe) or hosted anywhere.

Progress is saved to the browser's `localStorage`; the **Reset** button starts a
fresh week.

## How the simulation works

1. **Verify the backlog.** Pre-loaded coursework (ENT-101, ACC-110, COM-105) and
   internship deliverables start *locked*. Clicking a task opens a setup panel
   where the student confirms an estimated completion time, a priority level,
   and sees its hard deadline — only then does it become draggable.
2. **Deconstruct the elephant.** Major projects (Market Research Deck, Social
   Media Audit) can't be dropped onto a single day. Expanding the project card
   reveals sequential chunks (Research → Outline → Draft → Polish) that are
   scheduled individually — and the app warns when chunks are placed out of order.
3. **Drag & drop the week.** A Mon–Sun grid with Morning / Afternoon / Evening
   blocks, with fixed class sessions already locked in. Tasks move from the
   backlog into blocks, between blocks, or back to the tray.
4. **Guardrails give live feedback.**
   - **Independent Study Quota meter** — tracks coursework + deep-work hours
     against the 2–3 hours-per-class-hour standard (18–27h for the simulated
     9 class hours), with spawnable "Deep Work" study blocks to fill the gap.
   - **Overload / burnout alerts** — blocks glow red when over capacity, days
     flag burnout past 9 planned hours, and high-priority pile-ups and missed
     deadlines surface as warning banners.
5. **Check My Week** — a report card grades the plan across quota, verification,
   scheduling coverage, deadlines, capacity, and chunk sequencing, with a final
   verdict from 🏆 *Founder-grade week* to 🔥 *This week will eat you alive*.
