# Pipeline Foundation - Simple API

This repository now includes a minimal Flask API in `app/app.py`.

Quick start (from project root):

```powershell
python -m pip install -r requirements.txt
python app/app.py
```

The API listens on port 8000 by default.

Endpoints:

- `GET /` — welcome message
- `GET /health` — health status
- `GET /items` — list items
- `POST /items` — create an item (JSON body: `{ "name": "..." }`)

Example `curl`:

```powershell
curl -X POST http://localhost:8000/items -H "Content-Type: application/json" -d "{\"name\":\"example\"}"
curl http://localhost:8000/items
```
