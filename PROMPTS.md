# Prompt log — RoleReady

This document records the prompts and AI-assisted decisions used to build the RoleReady project for Task 1. It distinguishes the user's actual requests from the implementation decisions made in response. It does not invent additional verbatim prompts.

## AI tool used

**ChatGPT** was used in this conversation to read the supplied assessment, plan and create the project, refine the implementation, and prepare the documentation. No other AI tool or external AI API was used for this project. The app does not call an AI model when it runs: its score is produced by the transparent JavaScript rules described in `README.md`.

## User prompts that guided the work

### Prompt 1 — Read and explain the assessment

**Prompt (from the initial request, lightly shortened to remove repeated wording):**

> “Can you see the task? They give some tasks. I need to complete the task, and how will I complete? We can explore how to submit and which format can I submit, and can you read the task and do it? [...] Can you read deeply and what is the task, what is the requirement, and also how many tasks they will give you? Check it and do it, the task. How many tasks? Can you explain how many tasks, what we'll do, what is the requirement, how to submit?”

**Purpose:** Read the attached Task 1 PDF, separate its requirements from the email's general hiring process, and explain the project and submission format.

**Outcome:** Identified that this attachment describes one practical project in healthcare or technology and requires three submission items: a video of at least two minutes, prompt documentation, and a project link. The email mentions a later Python assessment, but that assessment was not attached.

### Prompt 2 — Re-read the assessment

**Prompt (verbatim):**

> “read the task 1”

**Purpose:** Re-state the actual Task 1 requirements directly and concisely.

**Outcome:** Confirmed that the deliverable should be one practical project rather than several separate projects, accompanied by the three required submission items.

### Prompt 3 — Build the project

**Prompt (verbatim):**

> “do it the the task”

**Purpose:** Move from explaining the task to creating a project that meets it.

**Outcome:** Selected the technology automation option and created RoleReady, a local job-posting triage and application-tracking prototype. The project fits the user's stated interest in Python, SQL, and automation without using real employer or applicant records.

## Project implementation brief

The following is a **summary of the working brief**, not a verbatim user message:

> Build one practical technology automation project for the assessment. Make it easy for a reviewer to run, demonstrate a real workflow, explain how the result is produced, and include the required prompt log and video guide. Be clear about synthetic data, limitations, and what AI did.

This brief was used to scope the project as a browser-based job search tool. It was deliberately kept self-contained: no installation, backend, account, API key, or external service is required.

## Refinements applied during implementation

These are implementation decisions made while responding to the requests above. They are **not separate verbatim prompts**:

1. **Make scoring inspectable.** Use a visible 100-point rubric: skills (35), location (15), experience (20), pay (10), and posting freshness (20). Show the component scores, matching skills, and review flags.
2. **Preserve human review.** Describe the score as a sorting aid, not a hiring prediction or automated rejection. Keep the original posting link available for manual verification.
3. **Protect example data.** Store entered roles in the browser's local storage and provide JSON import/export. Do not send role data to a service.
4. **Make the demo understandable.** Include synthetic examples with placeholder `example.com` links and label them as examples rather than live vacancies.
5. **Avoid unsupported personal claims.** Keep profile settings configurable and document that the sample profile values must be checked and updated before presenting.
6. **Disclose AI's role accurately.** State that ChatGPT helped create and refine the project while the runtime scoring itself is deterministic JavaScript, not an AI feature.
7. **Prepare the assessment outputs.** Include these instructions, the prompt log, and a video presentation script in the repository.

## Prompt iteration record

The interaction progressed in three substantive steps: assessment extraction, confirmation of the task requirements, and project implementation. The code and supporting files were then refined around score transparency, local data handling, synthetic examples, accurate profile disclosures, and clear AI-use limitations.

No separate prompts were sent to Claude, GitHub Copilot, or an AI API. The refinement list above records the concrete changes made in this ChatGPT workflow; it is not represented as a fabricated transcript of prompts that were never sent.

## Result and reproducibility

The final project is in the public repository at <https://github.com/hareeshmpro-max/roleready-task1>. Open `index.html` to run it. `README.md` explains setup, the scoring rubric, AI use, and limitations. `VIDEO_SCRIPT.md` provides a presentation outline of at least two minutes.
