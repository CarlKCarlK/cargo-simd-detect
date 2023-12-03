cargo-simd-detect
==========

Cargo command to report which SIMD levels your Intel/AMD CPU supports and are enabled.

Install
-------

```bash
cargo install cargo-simd-detect
```

Run
-------

```bash
cargo simd-detect
```

Output
-------

A short text report, for example:

```text
feature         width                   available       enabled
sse2            128-bit/16-bytes        true            true
avx2            256-bit/32-bytes        true            false
avx512f         512-bit/64-bytes        true            false
```

It was originally created for an [article about SIMD programming on *Medium*](https://medium.com/@carlmkadie). Expected in Dec 2023/Jan 2024.
