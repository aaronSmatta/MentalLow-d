# MentalLoad

A voice-first task manager for offloading the mental load. Dictate your to-dos, assign them to people, set due dates and flexible email reminders, and track recurring chores — all in a single self-contained HTML file.

Open `index.html` in a browser (Chrome or Edge recommended for live dictation).

## Features
- **Dictation → tasks** — speak via the Web Speech API (or paste text); auto-detects due dates ("by Friday", "tomorrow"), assignees ("assign to Sara"), priority, tags (`#home`) and recurrence ("every week").
- **People & assignment** — assign tasks to teammates with avatars.
- **Due dates & flexible reminders** — multiple before/after reminder rules that generate pre-filled email drafts to the assignee.
- **Recurring tasks** — daily/weekly/biweekly/monthly/yearly, defaulting to a 6-month horizon, expanded across the calendar and the Upcoming list day by day. Each occurrence is checked off (and reversible) on its own.
- **Calendar** — a modern month view on the dashboard and a full Calendar view; click any day to see its tasks in a dropdown.
- **Filtering** — by assignee and by tag.
- **Completion sound** — a short, satisfying chime on completion.
- **Dark mode** — persistent light/dark toggle.
- **Sync** — saves to Supabase out of the box (set up the tables once via the in-app ⚙ Settings SQL), with a local-storage fallback.

## Tech
Single HTML file: vanilla JS, Web Audio API, Web Speech API, and the Supabase JS client via CDN. No build step.
