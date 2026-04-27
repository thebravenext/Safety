# SafetyX Pro – AI-Powered CCTV Safety Monitoring Platform

SafetyX Pro by The Brave Next Ltd transforms existing CCTV/IP camera streams into a real-time industrial safety monitoring dashboard.

## Features
- Login / signup
- Camera source management
- Live stream preview
- PPE, truck inspection, and fire/smoke model modes
- Notifications, violation snapshots, and reports

## Setup
```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
uvicorn app.main:app --reload
```

Default login: `admin@example.com` / `admin123`

## Structure
```text
app/main.py
app/db/database.py
app/db/crud.py
app/models/models.py
app/schemas/schemas.py
app/services/video_processor.py
app/templates/
app/static/
scripts/
data/models/
tests/
```

## Production Notes
Change `SECRET_KEY`, hash passwords, use PostgreSQL, and do not push `.env`, videos, model weights, databases, or violation images to GitHub.
