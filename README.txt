VEL TECH HIGH TECH ENGINEERING COLLEGE PORTAL

Requirements: Node.js 18+ (Node 24 is okay)
Run in this folder:
  npm.cmd install
  npm.cmd start
Then open http://localhost:3000

Demo login:
  Admin: ID 4146, password 4146
  Student: VH14281, password 24VH14281
  Students may also log in using the five digits only, e.g. 14281.

Features:
- Student profile, attendance view, class/exam timetable, and mini-project submission.
- Student submissions are saved as Pending for admin review.
- Admin can add a mini-project directly; projects added by admin are automatically Approved.
- Admin can approve/reject student submissions and set attendance from 0 to 100%.
- SQLite database is created as portal.db in this folder on first run.

Troubleshooting:
- Keep the terminal running while using the website.
- This version fixes the student batch INSERT placeholder mismatch that caused Submit failed.
- If replacing an older project folder, back up its portal.db first and copy it into the new project folder to preserve existing records.

Security note: demo credentials and session secret are for local testing only. Change them before public deployment. The example timetable should be checked against the official college timetable.
