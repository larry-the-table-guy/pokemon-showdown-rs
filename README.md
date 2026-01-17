#### Hardware
6C/12T i7-9750h 16GB

All-core frequency capped to 3.60 GHz

#### Bench script:

```
cargo build --release --example test_unified
time ./target/release/examples/test_unified 1 2000 > /dev/null
```

For testing, I just diff the output of both.

#### Baseline (`796066f21b6a4d6a82f17f6b594f06dacbb0932b`)

```
real	0m16.770s
user	2m46.884s
sys	    0m0.089s
```

#### Head (`b2c9a9fed0f94b81b2f932a017e0bb3255b9a6b7`)

```
real	0m13.403s
user	2m13.320s
sys	    0m0.085s
```
