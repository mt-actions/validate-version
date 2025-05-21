# CHANGELOG

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).


## [3.0.0] - 2025-05-21

### Added
- CHANGELOG.md to track changes

### Changed
- Replace use of `mt-actions/assert` with `jackbilestech/semver-compare` for comparing versions
    - `mt-actions/assert` seems to have a bug such that `v0.10.0` is considered less than `v0.9.0`
- [BREAKING] Allowed comparison operators have changed.
    - `==` replaced with `=`
    - `!=` removed


## [2.0.0] - 2022-05-22

### Added
- Required `package_type` input parameter that specifies the type of package
    - Supports `python` and `csharp`

### Changed
- Use `mt-actions/get-version` for retrieving the version info


## [1.0.0] - 2022-04-30

### Added
- Initial release