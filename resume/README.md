# Resume & Cover Letter

This folder contains Halil's resume and a cover letter template in Markdown, plus a GitHub Actions workflow to export PDFs.

Files
- Halil-Aybar-Resume.md — main resume (Markdown)
- Cover-Letter-Template.md — quick‑edit template for applications
- resume.css — print stylesheet used by the exporter
- md-to-pdf.json — PDF options for headless Chrome

How to export PDFs (GitHub Actions)
1. Go to the Actions tab in this repo.
2. Run the "Export resume PDFs" workflow (workflow_dispatch).
3. When the run finishes, download the artifact named `resume-pdfs`. It contains:
   - resume/dist/Halil-Aybar-Resume.pdf
   - resume/dist/Cover-Letter-Template.pdf

Local export (optional)
- Requires Node.js 18+ and Chrome installed.
- Install once: `npm i -g md-to-pdf`
- Export: `md-to-pdf resume/Halil-Aybar-Resume.md --stylesheet resume/resume.css --basedir . --config-file resume/md-to-pdf.json --out-file resume/dist/Halil-Aybar-Resume.pdf`

Tailoring tips
- Mirror the job's exact keywords in Skills/Projects (e.g., TypeScript, Axios, Tailwind) if applicable to your experience.
- Keep to one page; prefer verb‑first bullets ("Built", "Implemented", "Designed").
- Put WTWR first; link both the live site and repos.