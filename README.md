# Weekly Time Planner

A browser-based weekly planner that connects to Google Calendar. View your week, add and remove time blocks, check for scheduling conflicts, and review planned time by category. This lets you plan your entire 168-hours of a week before plotting it in your live Google Calendar.

## Requirements

- A modern web browser
- Python 3, to serve the files locally
- A Google account and a Google Cloud project with the Google Calendar API enabled

## Setup

1. Keep `index.html`, `weekly-planner.html`, and `WSL_SquareLogo.png` in the same folder.
2. Start a local web server from that folder:

   ```powershell
   python -m http.server 8000
   ```

   On macOS or Linux, use `python3 -m http.server 8000` if `python` does not launch Python 3.
3. Open [http://localhost:8000/index.html](http://localhost:8000/index.html) and follow the on-page instructions to configure Google OAuth and download `client_id.txt`.
4. Save `client_id.txt` in the same folder as `weekly-planner.html`.
5. Open [http://localhost:8000/weekly-planner.html](http://localhost:8000/weekly-planner.html) and connect your Google Calendar.

Keep the server terminal open while using the planner. Do not open the HTML files directly from the filesystem; Google sign-in requires the local server origin to match the authorized JavaScript origin configured in Google Cloud.

## Privacy and terms

See [Privacy Policy](privacy-policy.html) and [Terms of Service](terms-of-service.html).

## Project files

- `index.html` — Google Calendar setup instructions
- `weekly-planner.html` — planner application
- `privacy-policy.html` — privacy information
- `terms-of-service.html` — terms of use
- `WSL_SquareLogo.png` — setup-page logo
- `client_id.txt` — locally configured Google OAuth client ID (created during setup)
