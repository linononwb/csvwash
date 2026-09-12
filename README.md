# csvwash

Small pandas pipeline that cleans messy CSV exports

## Features

- Chunked reading for files that do not fit in memory
- Writes a cleaning report next to the output
- Config-driven column renames and type casts
- Drops duplicates, trims strings, normalizes dates

## How to use

```bash
python pipeline.py raw.csv --config config.yaml --out clean.csv
```

## Getting started

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── config.yaml
├── pipeline.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
