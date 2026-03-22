# Model Governance Platform

A cloud-based platform for validating and auditing infrastructure financial models.

## What It Does

- Validates Excel financial models in seconds (not weeks)
- Detects structural issues (hard-coded assumptions, broken links, missing docs)
- Generates audit-ready reports that lenders trust
- Saves infrastructure funds £200k+ per refinancing cycle

## The Business

**Problem:** Infrastructure funds spend £200k and 10 weeks auditing models before refinancing.

**Solution:** Upload models → Get instant governance scores → Download reports.

**Revenue:** £8-15k/month per customer.

## Quick Start

### Local Development

```bash
# Clone repo
git clone https://github.com/your-username/model-governance.git
cd model-governance

# Backend
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py

# Frontend (in another terminal)
cd frontend
npm install
npm run dev
```

Open `http://localhost:5173`

### Deploy to Railway

1. Push to GitHub
2. Go to railway.app
3. Click "New Project" → "Deploy from GitHub"
4. Select this repo
5. Click Deploy
6. Wait 2-3 minutes for deployment

You'll get a live URL automatically.

## Architecture

- **Frontend:** React + Vite
- **Backend:** Python + Flask
- **Validation Engine:** openpyxl (Excel parsing)
- **Deployment:** Railway (cloud platform)

## Files

- `backend/app.py` - Validation engine
- `frontend/src/App.jsx` - User interface
- `requirements.txt` - Python dependencies
- `package.json` - JavaScript dependencies
- `docker-compose.yml` - Local Docker setup
- `Dockerfile` (backend & frontend) - Container configs

## Validation Checks

The platform scans for:
- Hard-coded assumptions
- Circular references
- Formula inconsistency
- Missing assumptions tab
- No version control
- Mixed data types
- Missing core sheets
- Audit readiness

## Pricing

- **Starter:** £500/month (5 models)
- **Pro:** £2,000/month (50 models)
- **Enterprise:** £8,000-15,000/month (unlimited)

## Support

For deployment issues, contact Railway support.
For code issues, check Flask and React documentation.

---

Built by Craig - BDO LLP | March 2026
