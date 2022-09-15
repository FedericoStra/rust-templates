# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com),
and this project adheres to [Semantic Versioning](https://semver.org).

## [Unreleased]

## [0.1.1] - 2022-09-15
### Added
- Template `lib`:
  - Make `docs.rs` automatically document the features required for each item.
  - Add basic module documentation.

## [0.1.0] - 2022-09-15
### Added
- Template `lib` to generate a basic library. Features:
  - `Cargo.toml` with name, author, description, license, repository;
  - `README.md` with description and badges (crates.io, docs.rs, repository, workflow, dependencies, license);
  - `CHANGELOG.md` automatically updated by `cargo release`;
  - `release.toml` to configure `cargo release`;
  - document all features on `docs.rs`;
  - GitHub workflow to check the library.

## [0.0.0] - 2022-09-15
Empty release.

[Unreleased]: https://github.com/FedericoStra/rust-templates/compare/v0.1.1...HEAD
[0.1.1]: https://github.com/FedericoStra/rust-templates/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/FedericoStra/rust-templates/compare/v0.0.0...v0.1.0
[0.0.0]: https://github.com/FedericoStra/rust-templates/releases/tag/v0.0.0
