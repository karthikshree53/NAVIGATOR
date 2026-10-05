AI SKILL GAP & CAREER NAVIGATOR - FIXED SETUP

1. Local:
   - Create .env from .env.example.
   - Put your real GEMINI_API_KEY in .env.
   - Install: pip install -r requirements.txt
   - Run: python app.py
   - Test Gemini: http://127.0.0.1:5000/gemini-status?test=1

2. Render:
   - Runtime: Python 3
   - Build Command: pip install -r requirements.txt
   - Start Command: gunicorn app:app
   - Environment -> add GEMINI_API_KEY with your real Google AI Studio key.
   - Save and deploy/redeploy.
   - Test: https://YOUR-SERVICE.onrender.com/gemini-status?test=1

IMPORTANT:
- Render does not read your local .env automatically. The real key must be entered in Render Environment Variables.
- Never commit a real API key to GitHub or put it in HTML/JavaScript.
- The app supports both GEMINI_API_KEY and GOOGLE_API_KEY.
- The dashboard/UI is kept the same as the supplied project.
