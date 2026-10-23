# Study Buddy: simulated Alexa+ skill

Track: Alexa+ (simulated experience path, no real device needed).

Study Buddy is a web app that simulates an Alexa+ voice assistant. You speak or type a request, and the app calls MCP-style tools (`create_study_plan`, `start_focus_timer`, `export_calendar`, `reschedule_plan`) to plan exam days , run a focus timer, or export the plan as a calendar (.ics) file. The tool call and result are shown live on screen, and the reply is spoken with the browser's speech synthesis.

## Run
Open `index.html` in Chrome. No install or internet needed. Use the Speak button for voice input (Chrome).

## Try
- "Plan my DSA exam in 3 days with 2 hours daily"
- "Start a 25 minute focus timer"

## Files
- `index.html`: the whole app (UI, intent parsing, tools)
- `LICENSE`: MIT

## Smart rescheduling
After making a plan, say "I missed day 2". The `reschedule_plan` tool moves the missed hours across the remaining days.
