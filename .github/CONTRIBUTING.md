# Contributing to EnvelopeSeal

Thanks for considering a contribution. EnvelopeSeal is an offline auditor: it
reads a key manifest and never touches a live key store.

## Development setup

- Python 3.11+. The package uses the standard library only.

```bash
python -m compileall -q src
python -m pytest -q
PYTHONPATH=src python -m envelopeseal validate samples/healthy.manifest
```

## Before you open a pull request

1. Compile and the full test suite must pass.
2. Every new check needs a fixture manifest, a test and a paragraph in the
   README explaining what a finding means.
3. Keep the package dependency-free.
