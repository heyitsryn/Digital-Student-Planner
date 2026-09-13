# Calm Campus Student Planner PWA

A responsive, offline-first planner inspired by the supplied reference PDFs. It uses an original name and implementation while preserving the requested calm cream, espresso, pink, pastel and editorial aesthetic.

## Features
- Home dashboard, timetable, tasks and quick capture
- ICS timetable import and free-block hint
- Assignments with checklists and progress
- Pomodoro timer and spaced-repetition flashcards
- Weighted grades and what-if projection
- Exams with countdown and readiness ratings
- Calendar, reading tracker, subjects and notes
- Wellness, water, goals and reminders
- Extracurricular clubs, roles, meetings and hours
- JSON backup/restore, new-term reset
- Automatic system theme plus manual light/dark/auto toggle
- Offline service worker and installable web manifest

## Run locally
Service workers require HTTP(S), not a file double-click. From this folder run:

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080`.

## Install on a phone
Deploy this entire folder to any HTTPS static host. Then open the HTTPS address on the phone and choose **Add to Home Screen** or **Install app** from the browser menu. Open it once while online so the app shell is cached.

## Data and privacy
Planner data is stored locally in the browser using localStorage. Use **More > Export** for backups and **Import** to restore. Clearing browser site data removes the planner data.

## Notes
- ICS import supports common VEVENT fields: DTSTART, SUMMARY and LOCATION. Complex recurring rules are not expanded.
- Cross-device sync and authentication require a backend and are intentionally not included in this offline static build.
