# rust-templates

> A collection of templates to be used with `cargo generate`.

[![GitHub](https://img.shields.io/static/v1?label=github&message=FedericoStra/rust-templates&color=brightgreen&logo=github)](https://github.com/FedericoStra/rust-templates)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/FedericoStra/rust-templates/build.yml?logo=githubactions&logoColor=white)](https://github.com/FedericoStra/rust-templates/actions/workflows/build.yml)
[![MIT license](https://img.shields.io/github/license/FedericoStra/rust-templates)](https://github.com/FedericoStra/rust-templates/blob/master/LICENSE)

These templates are supposed to be used with `cargo generate`:
- crate: <https://crates.io/crates/cargo-generate>
- guide: <https://cargo-generate.github.io/cargo-generate/index.html>

## Templates

### lib

Generate a basic library. Features:
- `Cargo.toml` with name, author, description, license, repository;
- `README.md` with description and badges (crates.io, docs.rs, repository, workflow, dependencies, license);
- `CHANGELOG.md` automatically updated by `cargo release`;
- `release.toml` to configure `cargo release`;
- enable all features on `docs.rs` (and document the features required for every item);
- GitHub workflow to check the library.

#### placeholders

- `gh_username`: GitHub username. The repository will be `{{gh_username}}/{{project-name}}`.
- `description`: description of the project.

### bin

Generate a basic binary. Features:
- `Cargo.toml` with name, author, description, license, repository;
- `README.md` with description and badges (crates.io, docs.rs, repository, workflow, dependencies, license);
- `CHANGELOG.md` automatically updated by `cargo release`;
- `release.toml` to configure `cargo release`;
- enable all features on `docs.rs` (and document the features required for every item);
- GitHub workflow to check the library and test the binary.

#### placeholders

- `gh_username`: GitHub username. The repository will be `{{gh_username}}/{{project-name}}`.
- `description`: description of the project.

## Release guide

This section is mainly intended for personal use, as a reminder to myself of the process of releasing a new version.

- Make sure `CHANGELOG.md` is up to date:
    + add under `## [Unreleased]` the relevant subsections among `Added`, `Changed`, `Deprecated`, `Removed`, `Fixed`, `Security`
    + change `## [Unreleased]` to `## [{{version}}] - {{date}}`
    + update links at the end:
        * `[Unreleased]: https://github.com/FedericoStra/rust-templates/compare/{{version}}...HEAD`
        * `[{{version}}]: https://github.com/FedericoStra/rust-templates/compare/{{previous_version}}...{{version}}`
- Tag the new version (remember to sign): `git tag -s v{{version}}`
- Push: `git push && git push --tags`
