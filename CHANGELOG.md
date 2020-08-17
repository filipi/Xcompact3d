# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- CHANGELOG.md by [@fschuch](https://github.com/fschuch).
- Xdmf writer included back, making easy to visualize the binary fields in other tools, by [@fschuch](https://github.com/fschuch).
- Sandbox flow configuration ([BC-Sandbox.f90](./src/BC-Sandbox.f90)), by [@fschuch](https://github.com/fschuch).
- Immersed boundary method for Scalar field(s), together with a new Lagrangian Interpolator for no-flux BC at solid/fluid interface, by [@fschuch](https://github.com/fschuch).
- Module Probes ([tools.f90](./src/tools.f90)), so now it can be used for any flow configuration, by [@fschuch](https://github.com/fschuch).

### Changed

- Enumeration, directory structure and filename format for binary outputs by [@fschuch](https://github.com/fschuch), details in [#3](https://github.com/fschuch/Xcompact3d/issues/3).

### Removed

- `subroutine VISU_PRE` ([visu.f90](./src/visu.f90)) is obsolete, since pressure is written at `subroutine write_snapshot` ([visu.f90](./src/visu.f90)), by [@fschuch](https://github.com/fschuch).

### Fixed

[Unreleased]: https://github.com/xcompact3d/Incompact3d/compare/dev...fschuch:master