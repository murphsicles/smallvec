# @collections/smallvec — Inline Small Vectors for Zeta

Auto-converted from [smallvec](https://crates.io/crates/smallvec) v2.0.0-alpha.12 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **Stack allocation** — stores up to N elements inline, zero heap allocations for small sizes
- **Automatic spilling** — transparently moves to heap allocation when capacity exceeded
- **Full Vec API** — push, pop, insert, remove, extend, resize, retain, dedup, drain, splice
- **IntoIter, Drain, Splice, ExtractIf** — iterator adapters matching standard Vec
- **Union/Intersection** — set-like operations on sorted smallvecs

## Usage
```zeta
use @collections/smallvec::SmallVec;

let mut v: SmallVec<[i64; 4]> = SmallVec::new();
v.push(1); v.push(2); v.push(3); v.push(4);  // stays on stack
v.push(5);  // spills to heap
```

## Stats: 2 source files, ~2,322 lines, 0 unsupported items

## License
MIT