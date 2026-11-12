# mojave

```
.
├── app.py             entry point: HTTP/2 client + static page server
├── requirements.txt   dependencies (hpack, optional header compression)
├── mojave.json        service manifest: runtime, start command, port, size
├── Procfile           web process fallback
├── Dockerfile         container build
└── .gitignore         ignored paths
```

Runtime reads `mojave.json`, runs `python app.py`, listens on `0.0.0.0:3000`.
