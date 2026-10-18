# CampusPulse updated batch portal

## Run in VS Code (Windows)
1. Install Node.js LTS.
2. Extract this folder and open it in VS Code.
3. Open Terminal in this folder.
4. Run:
   ```powershell
   npm install
   npm start
   ```
5. Open http://localhost:3000

## Demo accounts
- Admin ID: `4146`
- Admin password: `4146`
- Existing student: ID `VH14281`, password `24VH14281`

Student login pattern is `VH` + their 5-digit VH number, with password `24VH` + the same 5 digits. A student not yet in the database can request an account with that pattern; their first login is held pending admin approval. The admin approves it under **Student Login Requests**.

Students submit batch name, project title, and member details. Submissions stay pending until admin approves/rejects them. Approved batches are visible to students.

## Important
- The original “Innovative Assignment” section is not included in this replacement portal.
- This version uses SQLite, so data persists between browser sessions and is shared by users who connect to the same running server.
- `4146/4146` is a demo credential, not secure for a public deployment. Change it before deployment and set a strong `SESSION_SECRET` environment variable.
- This starter seeds only VH14281 from the provided material. Other student records are added as login requests and must be approved by admin; their names are not guessed from the photograph.
- For testing on phones, connect the phone and PC to the same Wi-Fi and open the PC's LAN IP with `:3000` (allow Node through Windows Firewall if prompted). Do not expose this demo server directly to the public internet.
