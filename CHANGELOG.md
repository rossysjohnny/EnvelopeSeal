# Changelog

All notable changes to EnvelopeSeal are documented in this file.
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Changed

- Rule wording is being reviewed for the next patch.

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
