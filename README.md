# FocusFlow

A minimal, single-file focus manager built for ADHD brains. No accounts, no installs, no distractions — just open `index.html` and work.

**[Try it live →](https://markdaily.github.io/focusflow-adhd/)**

---

## What it does

FocusFlow gives you three things in one quiet screen:

- A **focus timer** to time-box your work sessions
- A **task pool** to hold everything you need to do
- A **work log** where completed tasks land, timestamped

The idea is simple: pick a task, set a timer, drag the task over when you're done. Repeat.

---

## The three-column layout

| Column | What it's for |
|---|---|
| **Time** (left) | Timestamps for every item you've logged, with duration if you've marked it complete |
| **Work done** (middle) | Your running log of completed work — drag tasks here from the pool |
| **Task pool** (right) | Your to-do list. Add tasks, then drag them left to log completion |

---

## How drag-and-drop completion works

1. Add a task to the **Task pool** (right column) by typing and pressing Enter or clicking `+`
2. When you finish a task, **drag it left** into the **Work done** column
3. It appears in the log with a timestamp
4. Click the **circle checkbox** on any log entry to mark it fully complete — you'll hear a soft chime and see how long it took

---

## The timer

The header timer supports four quick presets — **25**, **50**, **15**, and **5** minutes — plus a custom duration field. Use it for Pomodoro-style focus blocks or whatever interval works for your brain.

- **Start / Pause / Reset** controls are always visible
- The arc ring fills as time runs out, turning red in the final minute
- When time's up, a gentle three-tone ding plays and a "Session complete" overlay appears
- Enable **Notify** to also get a browser notification when a session ends
- From the overlay you can start again immediately or dismiss and take a break

---

## Data persistence

Everything is saved automatically to your browser's `localStorage` — tasks and work log survive page refreshes and browser restarts. Nothing is sent anywhere. To clear data, use the **Clear** button in the Work done column, or open DevTools and clear `ff2_tasks` / `ff2_log`.

---

## Running it

No build step needed. Just open `index.html` in any modern browser:

```
open index.html
```

Or serve it locally:

```
npx serve .
# then visit http://localhost:3000
```

---

## License

MIT — do whatever you want with it.
