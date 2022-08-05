Changelog
===

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html), i.e. MAJOR.MINOR.PATCH (Breaking.Feature.Patch).

Types of changes:

- `Added` for new features.
- `Changed` for changes in existing functionality.
- `Deprecated` for soon-to-be removed features.
- `Removed` for now removed features.
- `Fixed` for any bug fixes.
- `Security` in case of vulnerabilities.

[Unreleased]
---

Major restructuring of the project to align with current qte77's SOTA project structure.

### Added

- App: `__version__.py`, `py.typed`
- Tools config: `.bumpversion`, `flake8`, `.markdownlint.yml`, `.pre-commit-config.yaml`

### Changed

- Project: `Pipfile`, `Pipfile.lock`, `pyproject.toml`
- App: `_version.py`
- git: `.gitignore`, `.gitmessage`
- gh-actions: `dependabot.yml`, `codeql.yml`, `links-fail-fast.yml`, `linter.yml`
- MDs to adopt markdownlint.yml

### Removed

- git: `ISSUE_TEMPLATE.md`

[0.7.0] - 2022-07-25
---

### Added

- README with definition of MVP's must, should, could and won't features

### Removed

- test/ because TDD only defined as MVP could and in contrast to current papermill pipeline and workflow

[0.6.0] - 2022-07-22
---

### Added

- Pipfile.lock for reproducible environment
- pyproject.toml as one file tools config and future packaging, e.g. with Poetry

### Changed

- .gitignore to not exclude pipfile.lock anymore
- README.md added develop TODOs
- app/app.py `logger`added for transition from `print()`
- app/helper/load_save_hf.py added TODO for decorators and get/setattr()

[0.5.0] - 2022-07-21
---

### Added

- .github/ISSUE_TEMPLATE.md

### Changed

- ./.gitignore to complement for dev-packages
- ./Makefile to add labels for testing and local setup and run with `pipenv`
- ./app/Pipfile to add dev-packages

### Removed

- ./app/.python-version because Pipfile `[requires]` specific python version

[0.4.0] - 2022-07-21
---

### Added

- `Pipenv` and modified `jupytext` labels in `Makefile`

### Changed

- Separated modules into `helper` and `model`
- Pydoc comments from `'` to `"`
- Generated current `app.ipynb` with label `py_to_nb` from `Makefile`

[0.3.0] - 2022-07-20
---

### Added

- Logic to  module `load_config`

### Changed

- Minor changes and renames

[0.2.0] - 2022-07-20
---

### Added

- Draft of module `loadSaveHF` for loading and saving Hugging Face components (models, datasets, tokenizer, metrics)
- Empty modules `loadConfig`, `inferModel` and `trainModel` for later use

### Removed

- Module `convertNbToPm` because conversion is done with `Makefile`

[0.1.0] - 2022-07-19
---

### Added

- Pipfile
- ./app/ipynb/*.ipynb
- ./app/__main\__.py

### Changed

- README.md

### Removed

- requirements.txt
- requirements-dev.txt
- Pipfile.lock
