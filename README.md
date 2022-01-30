# heaps
Experiments with different heaps implementations in Rust

# Benchmarks
I'm benchmarking two tasks, how much time it takes to push `0x10_000` values and then to pop all of them:
```
test kary_heap_16::push           ... bench:     199,016 ns/iter (+/- 76,944)
test kary_heap_16::push_and_pop   ... bench:   6,398,369 ns/iter (+/- 126,310)
test kary_heap_2::push            ... bench:     741,540 ns/iter (+/- 89,029)
test kary_heap_2::push_and_pop    ... bench:   4,527,586 ns/iter (+/- 100,620)
test kary_heap_4::push            ... bench:     408,292 ns/iter (+/- 3,606)
test kary_heap_4::push_and_pop    ... bench:   3,375,358 ns/iter (+/- 41,100)
test kary_heap_8::push            ... bench:     269,308 ns/iter (+/- 6,572)
test kary_heap_8::push_and_pop    ... bench:   4,101,809 ns/iter (+/- 72,508)
test my_binary_heap::push         ... bench:     767,787 ns/iter (+/- 118,916)
test my_binary_heap::push_and_pop ... bench:   4,463,074 ns/iter (+/- 145,382)
test std_heap::push               ... bench:     797,726 ns/iter (+/- 71,535)
test std_heap::push_and_pop       ... bench:   7,814,517 ns/iter (+/- 111,831)
test vectorized_binary_heap::push ... bench:     317,283 ns/iter (+/- 30,719)
```