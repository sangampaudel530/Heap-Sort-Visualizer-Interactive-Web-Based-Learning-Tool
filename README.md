
# Heap Sort Visualizer — Interactive Web-Based Learning Tool

An interactive, web-based Heap Sort visualizer with animations and step-by-step explanations. This repository hosts the front-end visualization files and a tiny Python server to run the demo locally.

## Highlights

- Clear animations for heap construction and heap sort phases
- Step-by-step controls (play/pause/step/back) in the UI
- Lightweight, dependency-free front-end (HTML/CSS/JS)
- Simple local server script (`server.py`) that opens your browser

## Files of interest

- `index.html` — main UI
- `visualizer.js`, `heap.js`, `app.js` — visualization and logic
- `styles.css` — styles
- `server.py` — small Python server (auto-opens browser)
- `screenshot_and_videos/` — screenshots and demo videos used in this README

## Screenshots

Below are the images found in `screenshot_and_videos/` included with the project.

![Screenshot 1](screenshot_and_videos/screenshot1.png)

![Screenshot 2](screenshot_and_videos/screenshot2.png)

![Screenshot 3](screenshot_and_videos/screenshot3.png)

If you add more screenshots or renamed files, update the paths above accordingly.

## Demo video

No demo video file was detected in `screenshot_and_videos/` at the time this README was generated. To include a video named `demo.mp4`, place it in `screenshot_and_videos/` and embed it like this:

<video controls width="720">
	<source src="screenshot_and_videos/demo.mp4" type="video/mp4">
	Your browser does not support the video tag.
</video>

Or link to a hosted video (YouTube/Vimeo):

[Watch demo on YouTube](https://www.youtube.com/)

## Quickstart (Windows PowerShell)

Prerequisites: Python 3.7+ (no extra packages required unless you use `requirements.txt`).

1) (Optional) Create a virtual environment and install dependencies:

```powershell
python -m venv .venv
; .\.venv\Scripts\Activate.ps1
; if (Test-Path requirements.txt) { python -m pip install -r requirements.txt }
```

2) Start the server and open the visualizer:

```powershell
python server.py
```

3) Alternatively, from Node-based workflows:

```powershell
npm run start
```

The server runs on port 8000 by default and will try to open your browser automatically.

## How to contribute

- Fork the repo, create a feature branch, and open a pull request. Keep changes small and focused.
- If you add screenshots or demo videos, put them under `screenshot_and_videos/` and update the README accordingly.

## Git/push notes (ensure `.gitignore` is applied)

If you already committed files that should now be ignored (e.g., `.venv/`), run these commands from PowerShell to reapply `.gitignore` before pushing:

```powershell
git rm -r --cached . ; git add . ; git commit -m "Apply .gitignore and update README" ; git push
```

This will remove cached files from the index while keeping them locally.

## Project contract (small)

- Input: user interacts with UI to generate arrays and control playback
- Output: animated heap construction and sorting visualizations with explanatory highlights
- Error modes: missing media files will simply not display; server port in use will show an error

## Edge cases to consider

- Empty array: UI should handle gracefully (no crash)
- Very large arrays: animations may be slow or crowded
- Browser compatibility: tested on modern Chromium-based and Firefox browsers

## License

MIT — see `LICENSE` (or add one if missing).

---

If you want, I can also:

- Auto-detect and embed any `.mp4`/`.webm` files in `screenshot_and_videos/` into this README
- Create a small `README-assets` script that generates the screenshots list automatically

Tell me which you'd prefer and I'll implement it.
