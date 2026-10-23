# Video presentation script — RoleReady

**Target length:** about 2 minutes 20 seconds. Record your screen while opening `index.html` and demonstrating the actions in brackets. Replace any profile details with accurate information before recording.

## Script

Hello, I’m Hareesh. For Task 1, I built RoleReady, a small technology automation project that helps organize a job search. The problem I chose is the repetitive work of reading postings, comparing them with a candidate profile, and keeping track of applications.

[Show the app header and explain the local privacy note.] I used ChatGPT to help scope the solution, draft the interface and browser logic, and refine how the score is explained. I chose it to accelerate implementation and iterate on the workflow. I reviewed the resulting code and kept the ranking logic simple and visible. The app does not call an AI model when it runs; it uses a fixed rubric, so a user can see how each score is produced.

[Click Load examples. Open the score breakdown for each example.] The score is out of 100: up to 35 points for skills, 15 for location, 20 for experience, 10 for pay, and 20 for posting freshness. The examples are synthetic and their example.com links are placeholders. Missing information gets a neutral score rather than being treated as a confirmed match.

[Add a sample role, or demonstrate changing a status.] A user can paste a job description, save it, inspect matched skills and review flags, and track it as to review, applied, interview, or closed. The dashboard summarizes the queue. The user can export a JSON backup and import it later. Job details stay in this browser unless the user exports them.

[Show the README or prompt log.] My prompt process started by extracting the assessment requirements, then I asked to complete the task. I refined the implementation around transparent scoring, human review, privacy, and clear disclosure of what AI did. The prompt document records those requests and the follow-up decisions.

One challenge was making a numeric score useful without making it look like a hiring prediction. I addressed that by displaying each score component, surfacing caution flags, and telling users to verify the original posting themselves. The project does not scrape sites, submit applications, or claim to make selection decisions.

This is the finished prototype. It turns a repeated comparison and tracking process into a lightweight local workflow, while keeping final decisions with the job seeker. Thank you.

## Recording checklist

- Confirm the `PROFILE` values in `index.html` match your own details, or clearly identify them as demo settings.
- Open the app in a browser and load examples before recording.
- Show at least one score breakdown, one status change, and the JSON export control.
- Keep the actual run between 2 and 3 minutes and make sure your voice is audible.
- Do not show personal email, phone, private job links, or browser-stored records you do not want to share.
