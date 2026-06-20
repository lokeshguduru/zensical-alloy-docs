# Zensical Alloy Docs

Public documentation for Zensical Alloy.

This repository consumes the published `zensical-alloy` theme package. It is
kept separate from the theme repository so the docs build behaves like a real
user project.

## Local Setup

```bash
python -m venv .venv
.venv/bin/pip install --upgrade pip
.venv/bin/pip install .
.venv/bin/zensical serve -a 127.0.0.1:8765
```

For unreleased theme changes, install the sibling theme repo instead:

```bash
.venv/bin/pip install -e ../zensical-alloy
```

## Checks

```bash
.venv/bin/zensical build
```

The `Deploy docs` workflow builds the site and publishes `site/` to GitHub
Pages on pushes to `main`.

