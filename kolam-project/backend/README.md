# Kolam Backend

FastAPI backend for kolam image analysis and generation.

## Local run

```bash
python -m pip install -r requirements.txt
python -m uvicorn main:app --host 127.0.0.1 --port 8000 --reload
```

## Render deploy settings

Use the backend folder as the service root.

- Runtime: Python, pinned by `runtime.txt` to Python 3.11.9
- Build command: `pip install -r requirements.txt`
- Start command: `uvicorn main:app --host 0.0.0.0 --port $PORT`

The requirements use `opencv-python-headless` because Render does not need desktop GUI OpenCV libraries.
