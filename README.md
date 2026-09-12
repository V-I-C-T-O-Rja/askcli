# askcli

Tiny streaming CLI for OpenAI-compatible chat APIs

Started as a weekend hack, grew on me.

## Usage

```bash
chatsh explain this error < error.log
cat diff.patch | chatsh review this diff
```

## Highlights

- Reads the prompt from args or stdin
- Works with any OpenAI-compatible endpoint
- Streams tokens as they arrive
- Model and system prompt via flags or env

## Installation

```bash
pip install -r requirements.txt
export OPENAI_API_KEY=sk-...
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── chatsh.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT. Do whatever you want.
