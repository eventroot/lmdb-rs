# lmdb-er (er... lmdb-rs)

Idiomatic and safe APIs for interacting with the
[Symas Lightning Memory-Mapped Database (LMDB)](https://www.symas.com/lmdb).

# origin and forks

This repo is a fork of [mozilla/lmdb-rs](https://github.com/mozilla/lmdb-rs), which has been archived.

Mozilla's fork was of [danburkert/lmdb-rs](https://github.com/danburkert/lmdb-rs), which,
while not archived, does not appear to have been maintained since 2017. Mozilla's documentation states
that their fork includes fixes for issues encountered by [mozilla/rkv](https://github.com/mozilla/rkv).

Mozilla's fixes are included in this repository's origin and the commit logs are intact as found.

## Building from Source

```bash
git clone --recursive git@github.com:eventroot/lmdb-rs.git
cd lmdb-rs
cargo build
```

## Tests

To run tests, pull the code and build from source.

Then:

```bash
cargo test
```

## Benches

While in the hands of Mozilla, some fundamental benchmarks were added. To run benchmarks, pull the code and build from source.

Then:

```bash
cargo +nightly bench
```

## Features

- [x] lmdb-sys.
- [x] Cursors.
- [x] Zero-copy put API.
- [x] Nested transactions.
- [x] Database statistics.
