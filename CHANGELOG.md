# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- ## [Unreleased] -->

## [0.2.0] - 2022-07-20

### Added

- Draft of module `loadSaveHF` for loading and saving Hugging Face components (models, datasets, tokenizer, metrics)
- Empty modules `loadConfig`, `inferModel` and `trainModel` for later use

### Removed

- Module `convertNbToPm` because conversion is done with `Makefile`

## [0.1.0] - 2022-07-19

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