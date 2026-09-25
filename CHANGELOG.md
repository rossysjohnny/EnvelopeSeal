# Changelog

All notable changes to EnvelopeSeal are documented in this file.
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Changed

- Rule wording is being reviewed for the next patch.
- A policy file format is being sketched for teams.

## [5.0.0] - 2026-08-22

### Added

- `blast --top N` to rank keys by reachable data keys in one call.

## [4.1.0] - 2026-08-15

### Added

- A `--policy` stub that reads expected wrap depths from a small file.

## [3.0.0] - 2026-07-14

### Changed

- Findings are ordered by severity, then by key id, in every output mode.

## [2.2.0] - 2026-06-09

### Added

- Per-key depth and wrap counts in the JSON report.
- A worked rotation example in the docs.

## [1.0.0] - 2026-05-26

### Added

- Stable contract: exit codes 0, 1 and 2, and the written manifest contract in
  `docs/FORMAT.md`.
- Cycle-safe reachability so a wrap cycle is reported once, not walked forever.

## [0.9.0] - 2025-06-24

### Added

- `blast` subcommand ranking keys by the number of data keys reachable below
  them.
- Rotation status against an explicit as-of date, with an exempt interval of 0.

## [0.8.0] - 2024-05-28

### Added

- Strength inversion detection: a wrap that maps a stronger key onto a weaker
  one is flagged with both sides quoted.

## [0.7.0] - 2023-04-18

### Added

- Named algorithm presets for the strength ordering, including the modulus
  family.
- `--as-of` is required for rotation checks; a missing date is a usage error.

## [0.6.0] - 2022-02-08

### Added

- JSON report with fixed keys, including per-key wrap counts and depths.
- `validate` and `rotation` subcommands.

## [0.5.0] - 2020-12-15

### Added

- Depth-first cycle detection over the wrap graph with the cycle path printed.
- Manifest parser for line oriented key and wrap records.

## [0.4.0] - 2019-01-22

### Added

- Wrap graph construction with per-key in and out degree.
- Orphan detection: wrapped keys with no encrypting key above them.

## [0.3.0] - 2017-12-19

### Added

- Rotation window rules with configurable intervals.
- Strict validation for key ids, algorithms and wrap records.

## [0.2.0] - 2016-10-11

### Added

- Strength ordering for symmetric and modulus based algorithms.
- `version` subcommand and the first report shape.

## [0.1.0] - 2015-05-26

### Added

- First release: key manifest model and the first integrity checks over a wrap
  list.
