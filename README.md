# topsheet-data

Static JSON data powering the Topsheet app: institutes, departments, and
per-department subject lists. Served via Vercel as plain static files —
no backend/API code, just JSON under `public/data/`.

## Endpoints (after deploy)
- `/data/institutes.json` — list of supported institutes
- `/data/departments.json` — BTEB department reference
- `/data/subjects/<deptCode>.json` — subjects for a department, semester-tagged

## Adding a new institute or department
Edit the relevant JSON file and push — Vercel redeploys automatically.
