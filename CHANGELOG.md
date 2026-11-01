# Changelog

## [v0.3.1](https://github.com/Aroy-Art/scalar_plug/compare/v0.3.0...v0.3.1) - 2026-11-01

### Security

* Update locked `plug_crypto` to 2.2.1 to fix [CVE-2026-105963](https://osv.dev/vulnerability/EEF-CVE-2026-105963), where the secret key base could be exposed in stack traces. `plug_crypto` is a transitive dependency and `mix.lock` is not shipped with the package, so run `mix deps.update plug_crypto` in your own application.

### Changed

* Update locked `floki` to 0.38.5 and `makeup` to 1.2.3
* Add the fork's copyright holder to the license, alongside Tuist GmbH
* Rewrite the changelog with versioned entries for the fork

### CI

* Add Dependabot configuration for Mix and GitHub Actions
* Update `actions/checkout` to v7 and `jdx/mise-action` to v4

## [v0.3.0](https://github.com/Aroy-Art/scalar_plug/releases/tag/v0.3.0) - 2026-09-09

First release of this maintained fork of [tuist/scalar_plug](https://github.com/tuist/scalar_plug).

### Changed

* **Breaking:** publish on Hex as `scalar_api_plug` instead of `scalar_plug`. Update your dependency to `{:scalar_api_plug, "~> 0.3.0"}`. The `ScalarPlug` module name is unchanged.
* Require `plug` `~> 1.20` (was `~> 1.16`)
* Require `floki` `~> 0.38` (was `~> 0.36.2`)
* Require `ex_doc` `~> 0.40` for development (was `~> 0.31`)
* Update package description, maintainers, and links for the fork

## Before the fork

History from [tuist/scalar_plug](https://github.com/tuist/scalar_plug), kept as originally generated.

* Add git cliff
* fix: loading failure when configuration is not passed by @pepicrft in [#6](https://github.com/tuist/scalar_plug/pull/6)
* Fix configuration by @pepicrft
* Set up CI by @pepicrft in [#5](https://github.com/tuist/scalar_plug/pull/5)
* Treat warnings as errors by @pepicrft
* Fix pipeline again by @pepicrft
* Fix CI pipeline by @pepicrft
* Remove Windows from the list by @pepicrft
* Add missing Erlang dependency by @pepicrft
* Enable experimental features by @pepicrft
* Delete Dagger by @pepicrft
* Initialize Dagger by @pepicrft
* Configure Renovate by @pepicrft in [#1](https://github.com/tuist/scalar_plug/pull/1)
* Add renovate.json by @renovate[bot]
* Add .vscode/settings.json and .vscode/extensions.json files to configure VSCode. by @pepicrft
* Finish the implementation of the package by @pepicrft
* Finish testing by @pepicrft
* Add tests by @pepicrft
