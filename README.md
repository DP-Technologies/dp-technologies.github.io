# DP Technologies — Website

Source code for the public website of **Dynamic Precision Technologies**,
published at [dp-technologies.ch](https://dp-technologies.ch).

Deployed via [GitHub Pages](https://pages.github.com) from the `/docs` folder
on the `main` branch.

## Structure

```
.
├── docs/                # Published website (GitHub Pages source)
│   ├── index.html       # The site (single-file, self-contained)
│   └── CNAME            # Custom-domain configuration
├── LICENSE              # Proprietary license — DP Technologies, all rights reserved
├── NOTICE.md            # Third-party attributions (HTML5 UP, fonts)
└── README.md            # This file
```

The repository root holds documentation and legal files only. Everything served
to the public lives under `docs/`.

## Local Preview

No build step is required. From the repository root:

```bash
# Python
python3 -m http.server 8000 --directory docs

# or Node (from inside docs/)
cd docs && npx serve .
```

Then open <http://localhost:8000>.

## Deployment

Pushes to the `main` branch deploy automatically to GitHub Pages.

GitHub Pages is configured to serve from:
- **Branch:** `main`
- **Folder:** `/docs`

The custom domain (`dp-technologies.ch`) is declared in `docs/CNAME` and must
remain in that file for the domain binding to persist across deploys.

## License

The contents authored by DP Technologies are proprietary — see [`LICENSE`](LICENSE).
Third-party components are attributed in [`NOTICE.md`](NOTICE.md).

## Contact

info@dp-technologies.ch
