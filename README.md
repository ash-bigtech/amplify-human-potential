# Humanoid — Full Stack Engineer Pre-Qualification Form

A self-contained, single-file HTML pre-qualification form for candidates applying to the Full Stack Engineer (Platform & Applications) role. Designed to be hosted on GitHub Pages with Formspree as the submission backend.

## Files

- `humanoid-prequalification.html` — the form itself. Fully self-contained (header image is embedded as a base64 data URI, so there are no external file dependencies).
- `recruiter-insights.md` — internal-only reference document. **Do not host this publicly or link to it from the form.** It explains what each question is designed to surface and how to read strong/weak answers.

## Setup

### 1. Connect Formspree

Open `humanoid-prequalification.html` and find this line near the top of the `<form>` tag:

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" id="prequal-form" method="POST">
```

Replace `YOUR_FORM_ID` with your actual Formspree form ID (the part after `/f/` in your Formspree dashboard URL).

### 2. Host on GitHub Pages

1. Push this repository to GitHub (public or private, both work with GitHub Pages on a paid plan; public repos work on the free plan).
2. In the repo, go to **Settings → Pages**.
3. Under "Build and deployment", set **Source** to "Deploy from a branch", choose your branch (usually `main`) and the root folder (`/`).
4. Save. GitHub will publish at `https://<your-username>.github.io/<repo-name>/humanoid-prequalification.html` — or rename the file to `index.html` if you want it at the repo's root URL.

### 3. Confirm Formspree is receiving submissions

Submit a test entry once live. Formspree requires confirming the first submission's email address before it starts forwarding subsequent ones to your inbox — check your Formspree dashboard if a test submission doesn't arrive.

## How the Fit & Availability Score works

Each submission includes two **hidden** fields that are only visible in your Formspree dashboard/email — never to the candidate:

- **Fit & Availability Score (internal)** — a single score like `44.0 / 52.0 (85%)`
- **Score breakdown (internal)** — the per-section breakdown that produced that number

The score is calculated entirely client-side in the browser at the moment of submission, from structured answers only:

| Component | Max points | Why |
|---|---|---|
| Right to work | 3 | Hard compliance gate |
| Location | 3 | Pipeline urgency |
| Onsite commitment | 3 | Non-negotiable for this role |
| Notice period | 2 | Sequencing |
| Standard proficiency (Python, JS, React, alt-framework) | 5 each | Self-rated skill |
| Differentiator proficiency (Rust, Golang) | 5 each, weighted ×1.5 | Rare, high-value skills for this role |
| Company-stage fit | 3 | Cultural fit proxy |
| Fast-paced environment comfort | 3 | Cultural fit proxy |

**Deliberately excluded from scoring:** the open-text paragraph answers (Infrastructure as Code, SDLC evolution, data governance & privacy, telemetry & observability). These require human judgement to assess — a candidate who pads an answer with buzzwords could otherwise outscore a concise, technically precise one. They are submitted as plain text for a person to read and judge directly; no automated score is attached to them.

The score is a **triage aid**, not a hiring decision. It's designed to help you sort a pile of submissions quickly by logistics fit and self-reported skill level — the actual hiring judgement still happens in the technical screen, informed by the paragraph answers and the recruiter insights document.

## Updating the form

The form is plain HTML/CSS/JS with no build step — open the file, edit, save, and push. All question text, scoring weights, and styling live in this single file.
