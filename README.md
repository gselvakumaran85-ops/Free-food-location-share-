```markdown
# Annadhanam Connect

A simple Streamlit app to share and discover free-food distribution locations.

Features
- Add "One Day" or "Daily" free food spots with start/end times.
- One-day spots auto-expire the morning after the last active day (06:00).
- Search by place name (uses Google Geocoding if GOOGLE_API_KEY set, otherwise OpenStreetMap Nominatim).
- Nearby results shown by distance from searched place/IP-approximate location.
- Persisted to a local `spots.json` file (for simple deployments).

Setup
1. Create a Python virtual environment:
   - python -m venv venv
   - source venv/bin/activate  (Linux/Mac) or venv\\Scripts\\activate (Windows)

2. Install dependencies:
   - pip install -r requirements.txt

3. (Optional) Set Google API key as environment variable for better geocoding:
   - export GOOGLE_API_KEY="YOUR_KEY"   (Linux/Mac)
   - setx GOOGLE_API_KEY "YOUR_KEY"     (Windows)

4. Run the app:
   - streamlit run app.py

Security note
- Do not commit your API keys into public repositories. Use GitHub Secrets or environment variables when deploying (Streamlit Cloud, VPS, etc).
```
