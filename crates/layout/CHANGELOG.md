# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.1](https://github.com/Dhirenderchoudhary/browser/compare/v0.0.1...v0.1.1) - 2026-06-21

### Added

- *(layout,cssom)* resolve percentage width + report used width/height
- *(cssom)* getComputedStyle reports used margins (resolved auto)
- *(layout)* resolve auto margins — `margin: 0 auto` block centering
- *(layout)* block-in-inline — blockify an inline element with block children
- *(cssom)* resolved used insets for positioned boxes + named window globals
- *(style,layout,engine)* CSS mask-image (the icon technique)
- *(style,layout,engine)* border-collapse + HTML presentational table attributes
- *(dom)* img width/height attrs + alt, naturalWidth/Height, dialog API, textarea/select .value
- *(engine,layout)* render inline <svg> (was a 0x0 box, zero graphics)
- *(forms)* render input/progress/meter as real widgets; label hit box
- *(layout,style)* real HTML table layout (was inline cells / vanishing rows)
- *(style,layout,paint)* block-level default rendering (margins, br, pre, hr, list markers)
- *(style,layout,paint)* default styling for inline text elements
- real Canvas 2D context (display list in JS, rasterized + composited by the engine)
- 279 HTML named entities + CSS ::before/::after generated content
- proper caret bar (not '|' glyph) + clickable <select> dropdowns (NSMenu)
- *(layout)* render <select> as a dropdown (selected option + ▾), not inline options
- *(css,style,engine)* linear/radial gradients, box-shadow, transform (translate/scale/rotate)
- checkboxes/radios, change/focus/blur/submit, hover events, text caret
- text form input — typing, value rendering, input/keydown events; fix load race
- *(css)* max/min sizing, line-height, text-transform, text-decoration, opacity, border-radius, logical props
- *(layout,engine,ffi,app)* clickable links (hit-test <a href> -> navigate)
- *(paint,layout,engine)* render <img> images (fetch, decode, blit)
- *(layout)* box-model layout with flexbox, grid, and positioning

### Fixed

- *(layout)* textarea renders its text content (was blank, ~4px tall)
- *(style,layout)* defensively skip out-of-bounds child ids in render walkers

### Other

- format workspace with rustfmt + make clippy clean (enforced in CI)
