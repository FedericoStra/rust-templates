# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com),
and this project adheres to [Semantic Versioning](https://semver.org).

## [Unreleased]

## [0.2.4] - 2025-04-24
### Changed
- Set `package.edition` to 2024 for templates `lib` and `bin`.

## [0.2.3] - 2025-04-24
### Added
- Reminder of common sections in `CHANGELOG.md` for templates `lib` and `bin`.

## [0.2.2] - 2024-04-09
### Changed
- Update GitHub CI actions to `actions/checkout@v4`, both in this project and in the individual templates.

## [0.2.1] - 2023-04-25
### Changed
- Allow manually running the GitHub workflow for templates `lib` and `bin`.

### Fixed
- Fix `cargo test` invocation in GitHub workflow for templates `lib` and `bin`.
  Remove the argument `--all-targets` otherwise the documentation is not tested.

## [0.2.0] - 2022-09-25
### Added
- Template `bin` to generate a basic binary. Features:
  - `Cargo.toml` with name, author, description, license, repository;
  - `README.md` with description and badges (crates.io, docs.rs, repository, workflow, dependencies, license);
  - `CHANGELOG.md` automatically updated by `cargo release`;
  - `release.toml` to configure `cargo release`;
  - document all features on `docs.rs`;
  - GitHub workflow to check the library.


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

[Unreleased]: https://github.com/FedericoStra/rust-templates/compare/v0.2.4...HEAD
[0.2.4]: https://github.com/FedericoStra/rust-templates/compare/v0.2.3...v0.2.4
[0.2.3]: https://github.com/FedericoStra/rust-templates/compare/v0.2.2...v0.2.3
[0.2.2]: https://github.com/FedericoStra/rust-templates/compare/v0.2.1...v0.2.2
[0.2.1]: https://github.com/FedericoStra/rust-templates/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/FedericoStra/rust-templates/compare/v0.1.1...v0.2.0
[0.1.1]: https://github.com/FedericoStra/rust-templates/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/FedericoStra/rust-templates/compare/v0.0.0...v0.1.0
[0.0.0]: https://github.com/FedericoStra/rust-templates/releases/tag/v0.0.0
