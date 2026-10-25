# Bookmark Server

In this exercise, you'll create a *bookmark server* or URL-shortening service,
similar to `TinyURL.com` or `goo.gl`, but with no persistent storage.

This server will accept a URL and a short name, check that the URL actually
works (returns an HTTP 200), then store it in a Python dictionary.

See `Bookmark_Server.py` for starter code and instructions.

## Running it

Python 3.15 (`.python-version`):

```bash
python3 -m venv .venv && .venv/bin/pip install -r requirements.txt
.venv/bin/python Bookmark_Server.py     # serves on $PORT, default 3100
.venv/bin/python test.py                # in a second terminal; needs internet (it fetches google.com)
```

CI runs the same on every push and pull request; Dependabot keeps `requests` and the actions current.
