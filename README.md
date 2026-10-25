# Brandorra Digital Dashboard — Phase 1 Starter

A responsive React + Vite dashboard prototype based on the supplied Brandorra Digital visual reference and requirements brief.

## Run locally

1. Install Node.js LTS if it is not already installed: https://nodejs.org/
2. Extract this folder and open it in VS Code.
3. Open Terminal in VS Code and run:

   ```bash
   npm install
   npm run dev
   ```

4. Open the local URL printed by Vite (usually `http://localhost:5173`).

## Included in this starter

- Responsive dashboard layout with the provided logo and brand-inspired colors.
- Sidebar navigation across dashboard, clients, projects, calendar, employees, payroll, attendance, recruitment/resumes, influencers, reports and settings.
- Sample KPI cards, revenue chart, campaign distribution, event list, client table, editable Kanban stages, calendar, HR/payroll views, candidate-source filters, searchable candidate list, resume preview panel, and influencer tracking.
- Demo add/edit modal patterns and toast feedback.
- Local resume selection workflow: select a PDF/DOC/DOCX file; PDF files can be opened in a browser preview. Files are not uploaded to a server and candidate details are not parsed or saved.
- Uploaded design reference image at `design-reference.png`.

## Important limitations

This is a Phase 1 frontend prototype with illustrative sample data. Forms and buttons demonstrate UI interactions but do not persist records. Resume parsing, file storage, live WorkIndia/Indeed/LinkedIn/Hirect ingestion, social APIs, authentication, RBAC enforcement, payroll calculations, encryption and backend/database integrations are not implemented. These require later phases, approved integrations, and security review.

## Design reference

Use `design-reference.png` as the visual comparison target. Use the official supplied logo in `src/assets/brandorra-logo.jpeg`.


### Dashboard promotional banner
The supplied Brandorra Digital wide banner is included at `src/assets/brandorra-banner.png` and displayed below the executive dashboard welcome header. It scales responsively on desktop and mobile.


## Recruitment workflow update (v6)

The recruitment prototype now supports session-level interactions:

- Add candidate records with role, experience, expected CTC, email, phone, skills, source platform, and hiring stage.
- Attach a local PDF, DOC, or DOCX file to a candidate. PDF files can be previewed in the browser; DOC/DOCX are listed by filename and can be downloaded.
- Search candidate records by name, role, skills, source, email, and experience.
- Filter by WorkIndia, Indeed, LinkedIn, Hirect, and hiring stage.
- Change hiring stage from the candidate table. Source cards, recruitment KPIs, and hiring pipeline counts update from the current candidate records.
- Open a detailed candidate/resume preview.

**Prototype limitations:** candidate data and object URLs remain in the current browser session and are not persisted to a database or uploaded to a server. Resume text is not automatically parsed. Live job-board integrations, authentication, access control, encrypted storage, and production security testing remain future phases.
