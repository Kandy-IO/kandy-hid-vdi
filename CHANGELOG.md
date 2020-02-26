# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). However, eLux packages also include a -X identifier, which represents the version of the eLux package

## 1.3.1-0 - 2020-01-31
### Added
- In Citrix VDI, filtering of known / supported devices has been removed. All HID devices found by the DLL are sent up to the kandy-hid-sdk for filtering and processing

## 1.2.0-2 - 2020-01-17
### Changed
- Rebuild of 1.2.0-1 to address a bug in the VDI Toolkit, which was built using the wrong version of RTC.DLL

## 1.2.1-0 2020-01-10
### Added
- Ability to disable the DLL (killswitch)

## 1.2.0-1 - 2019-11-04
### Added
- One of each supported type of HID device may now be connected to a Thin Client simultaneously.

## 1.1.0-1 - 2019-08-16
### Added
- Support for the Jabra Speak 710 in VDI mode

<!-- changelog possible fields:
### Added
### Changed
### Removed
### Deprecated
### Fixed
### Security
>