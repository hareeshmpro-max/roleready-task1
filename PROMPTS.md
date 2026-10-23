# Prompt documentation — RoleReady

This record includes the user requests that guided this project and the material refinement decisions made during development. ChatGPT was the AI tool used in this work. No other AI tool or external API was used. The app does not make runtime AI calls; its scoring is deterministic and visible to the user.

## Prompt 1 — Understand the assessment

> “Can you read the task and do it? … Can you read deeply and what is the task, what is the requirement, and also how many tasks they will give you? Check it and do it, the task. How many tasks? Can you explain how many tasks, what we'll do, what is the requirement, how to submit?”

**Purpose:** Read the provided Task 1 PDF, distinguish the assessment from the email's hiring process, and extract the project and submission requirements.

**Result:** Task 1 requires one practical healthcare or technology project, plus a video presentation of at least two minutes, prompt documentation, and a project link. The separate Python assessment is not in the supplied PDF.

## Prompt 2 — Request implementation

> “do it the the task”

**Purpose:** Proceed from explaining the assessment to completing a project.

**Result:** Choose the technology automation area and build RoleReady as a self-contained job search triage app. This draws on the Python/SQL/reporting automation experience described in the application email, without claiming that the project is an employer's live system.

## Refinement decisions made with AI assistance

These are implementation decisions and refinements, not additional user messages:

1. Make the score explainable using named components (skills, location, experience, pay, posting freshness), rather than presenting an opaque AI score.
2. Keep job data in browser local storage and provide JSON backup/restore so a reviewer can run the project without accounts, credentials, or an external service.
3. Make review flags visible and state that scores are prioritization aids, not hiring decisions.
4. Add synthetic sample roles so the interface can be demonstrated without using real people's data or suggesting fake vacancies are genuine.
5. Document that the profile values are configurable placeholders and should be confirmed before presenting.
6. Keep the app honest about AI use: ChatGPT helped build and refine the project; the app's runtime scoring is ordinary deterministic JavaScript, not an AI model.

## Prompt practice shown

The work demonstrates an iterative prompt workflow: first understand the assessment and its deliverables, then implement one focused project, then refine the scoring transparency, privacy, demo data, and disclosure of limitations. The complete conversation is available to the candidate as supporting context if the reviewer requests it.
