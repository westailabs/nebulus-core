# Changelog

All notable changes to **Nebulus Core** will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.1] - 2026-11-21

### Fixed
- Ship `intelligence/templates/*/config.yaml` in the sdist and wheel. Tag `v0.2.0`
  built as `nebulus_core-0.1.0` and omitted those files because setuptools
  package-data was not declared, so `list_templates()` / `load_template()` failed
  when the package was installed from a built artifact.
- Package version metadata now matches the release tag (`0.2.1` in
  `pyproject.toml` and `nebulus_core.__version__`). `v0.2.0` still advertised
  `0.1.0`.

## [0.2.0] - 2026-02-09

Tagged on `main` as `v0.2.0` (OverlordMemory canonical store and branch policy
docs). The built artifacts for that tag did not include the template YAML files
and reported version `0.1.0`.
