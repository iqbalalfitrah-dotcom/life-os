# Life OS — Android-ready prototype

This package is a polished PWA prototype designed for later Android packaging.

Features:
- Strava-inspired dark dashboard
- 05:00–22:00 schedule
- Daily checklist with persistence
- Progress ring
- 90-day goals
- Weekly scorecard
- Minimum Day mode concept
- English fluency goal
- Coding, job search, interview, workout and worship blocks
- Web Notification permission and in-page timers

## Important Android alarm limitation
A browser/PWA cannot reliably guarantee alarm delivery after the OS/browser fully terminates the process.
For the production Android version, package this project with Capacitor and add native local notifications/exact alarms.

Suggested production stack:
- Capacitor
- Android local notifications
- AlarmManager / exact alarm where legally/technically appropriate
- SQLite or local storage for offline data
- Optional Firebase Cloud Messaging only for server-triggered reminders
