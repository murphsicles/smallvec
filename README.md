# @collections/smallvec — Inline Small Vectors for Zeta

Auto-converted from [smallvec](https://crates.io/crates/smallvec) v2.0.0-alpha.12 via Dark Factory.

```zeta
use @collections/smallvec::SmallVec;

let mut v: SmallVec<[i64; 4]> = SmallVec::new();
v.push(1); v.push(2); // stays on stack
v.extend(0..100); // spills to heap when capacity exceeded
```

## Stats: 2 source files, ~2,322 lines, 0 unsupported
