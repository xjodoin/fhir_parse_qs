# Changelog

Notable changes to the project are (hopefully) documented in this file.

Attempts are made to confirm to semantic versioning.

## [Unreleased]

## [0.10.0] - 2025-09-15
### Changed
- Distribution renamed to `fhir-qs-parser` (module import remains `fhir_parse_qs`).
- Packaging modernized to `pyproject.toml`; added uv configuration and dependency groups.
- CI updated to Python 3.8–3.12; uses `uv` for sync/test/build; updated GitHub Actions to latest.
- Dependency bump: `pendulum` to `>=3`.

### Fixed
- NameError in `Search.valid_modifier` for reference modifiers (use `self.supported`).

### Notes
- If publishing from GitHub Actions, ensure `PYPI_API_TOKEN` is defined in repository secrets for the new PyPI project name.
