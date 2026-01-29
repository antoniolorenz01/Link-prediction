# Contributing

Thanks for your interest in contributing!

## Ways to contribute

- Fix typos or improve explanations in the notebook / README
- Add alternative baselines or models
- Improve reproducibility (seeds, configs, logging)
- Add scripts that turn the notebook into a runnable pipeline

## Development setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Notes:
- **PyTorch** and **PyTorch Geometric** can require platform-specific wheels. If installation fails, install them following their official guides, then retry.

## Notebook workflow

- Keep the notebook readable and narrative-driven (clear section headings, short code cells).
- Prefer deterministic runs when possible (set seeds).
- Avoid committing large generated artifacts (datasets, model checkpoints). The `.gitignore` includes common artifact folders/files.

## Submitting changes

1. Create a branch
2. Make your changes
3. Open a pull request with a short description and, if relevant, screenshots of notebook outputs

