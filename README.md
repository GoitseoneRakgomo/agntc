# AGNTC Landing Page

A responsive Flask landing page for AGNTC, prepared for deployment on Vercel.

## Requirements
- Python 3.10+
- Git
- A Vercel account

## Run locally (Windows PowerShell)

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
flask --app app run --debug
```

Open http://127.0.0.1:5000

If PowerShell blocks activation, run the app without activating the environment:

```powershell
py -m pip install -r requirements.txt
py app.py
```

## Deploy to Vercel

1. Push this project to a GitHub repository.
2. In Vercel, select **Add New → Project** and import the repository.
3. Keep the project root as the repository root.
4. Vercel should detect the Python function from `app.py` and use `vercel.json`.
5. Deploy.

No custom build command is required. The Flask application is exposed as `app` in `app.py`.

## Before publishing
- Confirm the contact email: `agenticsolutionsltd@gmail.com`
- Add the official company website URL when available.
- Replace any placeholder social links with the correct AGNTC profiles.
- Add real client testimonials, case studies and certifications only when approved and verifiable.

## Project structure

```text
agntc-landing-page/
├── app.py
├── requirements.txt
├── vercel.json
├── templates/
│   └── index.html
└── static/
    ├── css/styles.css
    └── js/main.js
```
