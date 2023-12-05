cargo-simd-detect
==========

Cargo command to report which SIMD extensions your Intel/AMD CPU supports and are enabled. It should be installed in Rust nightly.

Run
-------

```bash
# assumes rustup override set nightly
cargo install cargo-simd-detect --force
cargo simd-detect
```

To see changes to "enabled", you must re-install with `cargo install cargo-simd-detect --force`.

Output
-------

A short text report, for example:

```text
feature         width                   available       enabled
sse2            128-bit/16-bytes        true            true
avx2            256-bit/32-bytes        true            false
avx512f         512-bit/64-bytes        true            false
```

Created for an [article about SIMD programming on *Medium*](https://medium.com/@carlmkadie) that will be published in Dec 2023/Jan 2024.
