# etlpocket

Small pandas pipeline that cleans messy CSV exports

## What it does

- Config-driven column renames and type casts
- Chunked reading for files that do not fit in memory
- Drops duplicates, trims strings, normalizes dates
- Writes a cleaning report next to the output

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
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
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

## Acknowledgments

- README structure inspired by popular OSS templates
- Thanks to everyone opening issues with ideas

## License

MIT. Do whatever you want.
