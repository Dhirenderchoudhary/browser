# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.1](https://github.com/Dhirenderchoudhary/browser/compare/v0.1.0...v0.1.1) - 2026-06-21

### Added

- *(dom,js)* namespace lookup, DocumentType/PI, CSS.escape selector parsing, Attr/NamedNodeMap, DOMTokenList reflections
- *(wpt-runner)* dark-mode report (@media prefers-color-scheme) + multi-area runs
- *(wpt-runner)* emit an HTML results report (viewable in our own browser)
- *(wpt-runner)* in-process Web Platform Tests harness runner

### Fixed

- *(css)* unterminated string ends at newline (bad-string recovery); feat(wpt-runner): .sub substitution + .headers

### Other

- *(wpt)* include /common/ in the sparse checkout ([#14](https://github.com/Dhirenderchoudhary/browser/pull/14))
- format workspace with rustfmt + make clippy clean (enforced in CI)
- *(wpt-runner)* skip tentative WPT tests (tentative/ dirs + *.tentative.* files)
