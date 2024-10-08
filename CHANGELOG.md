# Changelog

All notable changes to spreadcat.matterhorn will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [v2.2.0] - 2024-10-08

### Fixed

- Updated the variable documentation in `./defaults/main.yml`, fixed some typos and added
  clarification where necessary.

### Added

- Added `./meta/argument_specs.yml` to make sure the variables are correctly defined and
  documented.

## [v2.1.0] - 2024-10-04

### Fixed

- Fixed an invalid value in the configuration test.

### Added

- The file `argument_specs.yml` has been added to validate the input variables.

## [v2.0.0] - 2024-09-25

### Fixed

- The role is now idempotent.

### Added

- The requirement `bzip2` is now installed when missing during the role execution.
- The role deploys a ansible fact onto the target system to establish the installation state and version of matterhorn.
- Testing scenarios for the different installation situation have been added.

### Changed

- The installation behaviour has been changed. The role now installes the latest version released from the source
  repository. By default existing installation will not be updated unless the parameter `matterhorn_state` has been set
  to `latest`.
- Updated the linting rules for Yamllint and markdown-lint.

### Removed

- The parameter `matterhorn_release_url` has been removed.

## [v1.0.1] - 2024-09-17

### Added

- Replacing the existing config file will create a backup file to preserve previous settings.
- Markdown-lint default configuration for linting markdown files.

### Fixed

- There was a typo in the `defaults/main.yml` file that caused a fail when the current user was used for installation.

## [v1.0.0] - 2024-09-17

### Added

- Initial version.

...
