# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this project does adhere to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]
- Auto-Test Generator

## [1.5.0] - 2019-06-20
### Added
- [Dockerfile](Dockerfile) Add Dockerfile 
- Support docker app, wb, pywb, ftw_compatible_tool

## [1.4.1] - 2019-05-24
### Added
- [Travis](https://travis-ci.org/microsoft/WAFbench) Add continuous integration travis
- [pytest](./tests/) Add pytest file

## [1.4.0] - 2019-04-30
### Added
- [ftw_compatible_tool](./ftw_compatible_tool) a test framework of WAF
- [regression-test](./util/regression-test) Test cases can be used by ][ftw_compatible_tool](./ftw_compatible_tool) or [pywb](./pywb)

### Changed
- [wb](./wb/wb.c) 
    - Fixbug: to send/receive packages that contain binary data will fail
    - Fixbug: program will exit if the connect timeout
- [pywb](./pywb) add support for binary package


## [1.3.0] - 2018-08-24
### Added
- [pywb](./pywb) an enhanced tool to wb.

### Changed
- [Makefile](./wb/Makefile) add argument -rf to rm for make clean
- [Makefile](./wb/apr/Makefile) modify apr download url to a stable
- [example](./example) change sample folder to example folder


## [1.2.1] - 2018-08-01
### Added
- [wb.c](./wb/wb.c) Add a feature to forcefully assert the "Connection: close" for each request packets.

### Changed
- [wb.c](./wb/wb.c) Polish the output


## [1.1.0] - 2018-08-01
### Added
- [wb.c](./wb/wb.c) Add a feature of sending requests ordered by timestamp

### Removed
- [wb.c](./wb/wb.c) Remove useless comments

### Fixed
- [wb.c](./wb/wb.c) Fix compiling warning
- [wb.c](./wb/wb.c) Fix typo
- [wb.c](./wb/wb.c) Fix crash bug of unspecified log
- [wb.c](./wb/wb.c) Fix carsh bug of sending huge packets


## [1.0.0] - 2018-07-16
### Added
- [README.md](./README.md) describes WAF Bench tool suits project.
- [CHANGELOG.md](./CHANGELOG.md) to track changes.
- [wb](./wb/README.md), a superset of [ab](https://github.com/CloudFundoo/ApacheBench-ab) to make benchmarking WAF more easily.
- `./sample` to show demos of WAF Bench tool suits. Currently, it only has examples for wb.

### Changed
- Revise the Makefile for apr and wb to support wb new feature.
