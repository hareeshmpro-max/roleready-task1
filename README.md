# RoleReady — AI Growth & Automation Associate, Task 1

RoleReady is a small technology workflow tool for prioritizing job postings. Enter a role and candidate profile details, get a transparent match score with reasons, and track the application pipeline. It addresses the repetitive work of comparing postings and maintaining a job application queue.

## Run it

1. Open `index.html` in a current browser. It needs no installation, account, API key, or server.
2. Select **Load examples** to see two synthetic roles. They use `example.com` links and are not real vacancies.
3. Add a real posting by pasting its details into the form. The score is recomputed as you edit fields and save.
4. Open **See score breakdown & review flags** to inspect the score components and cautions. Change a role's status to track progress.
5. Use **Export** to save a JSON backup or **Import** to restore one. Data stays in the current browser's local storage unless exported.

## Scoring

The fixed, visible rubric totals 100 points: profile skills (35), target location (15), requested experience (20), listed compensation (10), and posting freshness (20). Unknown posting dates receive a neutral 10 freshness points; missing pay receives a neutral 5 points; unknown experience receives 10 points. A small set of explicit rules creates review flags, such as a location outside the configured profile. This is a sorting aid, not an AI hiring decision or a prediction of selection.

The demo profile is configured in the `PROFILE` object near the bottom of `index.html`. Update its years, target locations, skills, and minimum pay to match your own confirmed profile before presenting. The current values are examples and should not be described as verified personal facts unless you confirm them.

## AI use and limitations

ChatGPT assisted with scoping, UI/code drafting, iteration on the scoring rubric, and preparation of the prompt log and presentation script. The working app itself uses ordinary browser JavaScript and a deterministic rubric; it does not call an AI API, scrape job boards, log in, submit applications, or send data to a service. The user remains responsible for checking each original listing and all eligibility requirements.

## Submission package

- `index.html`: runnable project.
- `PROMPTS.md`: prompt history and iteration record.
- `VIDEO_SCRIPT.md`: a two-minute-plus presentation guide.

To share a project link with the assessment team, publish this folder to a GitHub repository or put it in Google Drive and enable access for the reviewers. The local folder and ZIP are not public links by themselves.
