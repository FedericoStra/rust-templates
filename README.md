# rust-templates

> A collection of templates to be used with `cargo generate`.

[![GitHub](https://img.shields.io/static/v1?label=github&message=FedericoStra/rust-templates&color=brightgreen&logo=github)](https://github.com/FedericoStra/rust-templates)
[![MIT license](https://img.shields.io/github/license/FedericoStra/rust-templates)](https://github.com/FedericoStra/rust-templates/blob/master/LICENSE)

These templates are supposed to be used with `cargo generate`:
- crate: <https://crates.io/crates/cargo-generate>
- guide: <https://cargo-generate.github.io/cargo-generate/index.html>

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
