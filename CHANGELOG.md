# Changelog

All notable changes to claude-codex-pair are documented here. Releases follow
[Semantic Versioning](https://semver.org/spec/v2.0.0.html) while the project is pre-1.0.

## [Unreleased]

## [0.2.0] - 2026-08-27

### Added

- Test-count baselines and test-diff integrity checks that reject weakened assertions,
  deleted coverage, tautological expectations, and mocked-out behavior.
- A real run gate driven by a fresh agent that has not read the implementation diff.
- CI checks for the installer, skill frontmatter, opt-in guarantees, and relative links.
- Explicit installation safety checks for empty or root destinations.

### Changed

- The green gate now requires evidence beyond an agent's claim that tests pass.
- Runtime scenarios are written before implementation and verified with verbatim output.
- GitHub Actions use the current Node 24-based checkout runtime.

## [0.1.0] - 2026-07-27

The first tagged release: opt-in `/pair` and `/pair-review` skills, a sandboxed Codex
implementation handoff, fresh-context Claude review, bounded fix loops, deterministic
project gates, and one commit per green checkpoint.

[Unreleased]: https://github.com/hyj28/claude-codex-pair/compare/v0.2.0...HEAD
[0.2.0]: https://github.com/hyj28/claude-codex-pair/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/hyj28/claude-codex-pair/releases/tag/v0.1.0
