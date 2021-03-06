# ChangeLog

## 0.4.3

- only check if stderr is a tty for the auto color choice, all other
  choices pass through without modification
- bump termcolor to 1.0

## 0.4.2

- add the ability to not show logging levels via `.show_levels()`
- auto color choice (the default) will now disable colors if stderr
  is not connected to a tty by default

## 0.4.1

### Added

- Support millisecond timestamp resolution

## 0.4.0

### Added

- Timestamp now implements FromStr to make arg parsers quicker to implement
- Added a StructOpt example to the crate documentation and examples

### Changed

- Improved clap example and added Timestamp support
- Full use and depend on log 0.4.1.

## 0.3.0

### Added

- a large example under examples to detail how module level logging
  works

### Changed

- bump minimum Rust version to 1.16.0
- allow all log 0.3.x releases
- fix situations where including `a::b` also included `a::baz`

## 0.2.4

### Changed

- pinned log to 0.3.8 or older to retain Rust 1.13.0 support

## 0.2.3

### Added

- clap example
- support timestamps with microsecond and nanosecond granularity

### Changed

- improved performance (https://github.com/cardoe/stderrlog-rs/pull/2)
- improved docopt example in README
- migrated from time to chrono

### Thanks

- Thanks to Zachary Dremann <dremann@gmail.com> for the performance
  improvements and the nudge to improve the docs.
