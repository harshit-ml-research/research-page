# Research journal

Static HTML research journal for `research.hsbhandari.dev`.

## Pages

- `index.html`: research overview.
- `completed.html`: completed IEOR, IIT Bombay smoke experiments and failure analysis.
- `current.html`: internal Param17B SFT evaluation preparation.
- `compute.html`: where experiments ran and what is currently verified.

Build with Python's standard library:

```sh
python3 build.py
python3 -m http.server 8765 --bind 127.0.0.1
```

Open http://127.0.0.1:8765 locally. No package installation, external fonts, scripts, or build service is required. HTML pages are checked into Git so any static host can serve them directly.

Update the research copy in `build.py`, rebuild, and review the generated pages. Internal access docs and private operational data are excluded. Current SFT work is accurately labeled as preparation; the site claims no new benchmark scores.

GitHub Pages serves the main branch from the repository root. The custom domain is configured as `research.hsbhandari.dev` and persisted in `CNAME`. DNS must point the `research` CNAME to `harshit-ml-research.github.io`; certificate provisioning follows DNS validation.
