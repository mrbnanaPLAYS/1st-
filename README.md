# 1st

## Run the app

1. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```

2. Start the server:
   ```bash
   python app.py
   ```

3. Visit the app:
   ```bash
   curl http://127.0.0.1:5000/
   ```

   You should see a JSON response with a greeting message.

## How it works

The app is a minimal HTTP service defined in `app.py` using the Python standard library:

- A `BaseHTTPRequestHandler` subclass handles GET requests.
- The `/` route returns JSON with a greeting and a quick usage hint.
- Running `python app.py` starts the server on port `5000`.
