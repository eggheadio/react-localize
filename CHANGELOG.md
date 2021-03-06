# Change Log
All notable changes to this project will be documented in this file. This project attempts to adhere to [Semantic Versioning](http://semver.org/). We also try to use [http://keepachangelog.com/](http://keepachangelog.com/) formatting for this file to make it easier to update and read.

## [Unreleased]
_(add items here to be added to future release)_

## 2.0.0 2017-02-14
### Added
- Support for `.eslintrc`, code clean up to get `src/` directory passing new rules
- Connected components can now log warnings out when `_localizeDebug` is set, and will
always be passed a safe to invoke function regardless of a missing context function.

### Changed
- Localization Connector now behaves more like redux `connect()` in that it passes
`localize()` as a prop to components now, removing the need for components to access
context.
- Project now uses `save-exact` for installed dependencies

## 1.1.1 2016-08-02
### Fixed
- Bug to handle passing `null` to `localize('label', null)` more gracefully

## 1.1.0 2016-08-02
### Added
- Support for peerDependency `react@^0.14.6 || 15.x`
- Changelog formatting for better release tracking

### Changed
- Repo files (.gitignore, README.md)

### Fixed
- Bug causing `[]` to show at end of messages using `<Text />` introduced [here](https://github.com/sprjr/react-localize/blob/fde285cb2392194db7712a619f040b0c21daecaf/src/Localization.jsx#L35).

## 1.0.0
Intial release of `<Localization />` wrapper and `<Text />` helper components for looking up keys in a message bundle and localizing text. Includes interpolation, custom rendering options, and context helper function.
