# Lodestar

A single-file, offline personal planner for work and life. One HTML file. No server, no accounts, no internet needed.

Open `Lodestar.html` in your browser. All your data stays private on your device, stored in your browser's local storage. Share the file with others; their data remains completely separate and private to their own browser.

## What it does

**Kanban board** with cumulative time horizons — sort tasks across Total Work, 3 Months, This Month, This Week, Today, and Archive. Tasks are organized under pillars (projects), each with its own color and progress tracking.

**Day timeline** — drag Today tasks onto a 07:00–20:00 calendar view to block time. Resize blocks in 15-minute steps. Default durations respect energy labels (deep focus, shallow work, default 60min).

**Focus timer** — wall-clock-based Pomodoro or Flow mode. Logs focus time by task and date. Never undercounts, even if the browser tab is backgrounded.

**Habits tracker** — monthly grid calendars with streak counting and consistency %. Link habits to projects or leave them standalone.

**Daily journal** — one entry per day with a reflection prompt.

**Quick-capture inbox** — jot ideas anytime, sort them into projects later.

**Insights view** — focus time per project, per day, last 7 days.

**Evening planning** — at 17:15, a banner reminds you to export your day and plan tomorrow. Export/import your data by date to move between devices.

## Design principles

- **Calm and minimal.** Dark theme by default (charcoal + sage), light theme available. No busy dashboards. No notifications.
- **Offline and private.** Everything lives in your browser. No cloud, no syncing, no telemetry.
- **Single file.** No build step, no dependencies. Drag it to your device, open it, use it.
- **Hierarchy matters.** Tasks nest under projects (pillars). Subtasks nest under tasks. But nesting stays in Total Work; scheduled columns (This Week, Today) show a flat view to keep focus tight.
- **Drag doesn't change hierarchy.** Dragging a task to a different time horizon just reschedules it. To change where a task lives, you move its pillar via the task detail panel.

## How to use

1. Download `Lodestar.html` to your device
2. Open it in a browser (Brave, Chrome, Firefox, Safari all work)
3. You'll see sample seed data — rename domains/pillars to your own projects
4. Drag tasks between columns to schedule them
5. Click a task to add details: deadline, priority, focus time block, notes
6. Open the calendar view to time-block your day
7. Run the focus timer attached to any task
8. At day-end, export your state and import it on another device if you want to sync manually

## Themes

Two built-in themes. Toggle with the ☾/☀ button in the top right.

- **Dark** (default): Soft charcoal background, warm sage + dusty accent colors
- **Light**: Paper tones, easy on the eyes in bright daylight

## Habits & identity

Every project has an identity statement (optional) and a "votes cast" counter that tracks completed tasks and habit days. An aspiration ticker cycles through four rotating phrases tied to each project, once per day.

## Deadlines, energy tags, priority

- Set a deadline on any task (task detail panel)
- Tag tasks as deep focus or shallow work; the timer and day-timeline respect this
- Mark a task as "Today's priority" (★) to stand out in the Today column

## Undo / Redo

Every action is undoable. Use Ctrl+Z / Ctrl+Shift+Z (Cmd+Z on Mac).

## Data & export

Your data is stored in your browser's local storage under the key `myplanner.v3`. You can export a JSON backup anytime. To move data between devices, export from one, then import into another.

No automatic sync. By design — your data stays on your device unless you explicitly share it.

## License

Lodestar is free to use for personal, non-commercial purposes. No one may sell Lodestar or build a commercial business on it without the author's permission. The author retains the right to commercialize Lodestar at any point in the future.

For the full license terms, see `LICENSE.md`.

## Fork & tinker

You're welcome to fork this and modify it for your own use. If you have ideas, bug fixes, or accessibility improvements, you're invited to share them. Larger feature requests or design changes are best discussed as issues first.

## Built with

- HTML, CSS, JavaScript (no frameworks, no build step)
- Plain browser APIs (`localStorage`, `Date`, `fetch` for import/export)
- [Google Fonts](https://fonts.google.com) for typography

## Inspired by

- Atomic Habits (identity layer, votes cast)
- Getting Things Done (inbox, multi-level hierarchy)
- Cal Newport's time-blocking and deep work principles
- The pomodoro technique

---

Made for people who think in projects, value deep work, and want their planner to stay calm and out of the way.
