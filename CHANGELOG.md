# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## 0.1.3 - 2019-04-25
### Added
- A consuming iterator.
- Implemented `IntoIterator` for `&Bitvec` and `BitVec`.

## 0.1.2 - 2019-04-25
### Added
- `CHANGELOG.md`
- `BitVec::with_capacity()`
- `BitVec::from_bools()`
- Implemented the following:
  - `From<&[bool]>` for `BitVec`
  - `From<&Vec<bool>>` for `BitVec`
  - `From<Vec<bool>>` for `BitVec`
  - `From<&BitVec>` for `Vec<bool>`
  - `From<BitVec>` for `Vec<bool>`
- Specialized `Iterator` methods `size_hint`, `count`, `nth`, and `last` for
  performance.
