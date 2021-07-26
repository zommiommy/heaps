# heaps
Experiments with different heaps implementations in Rust

# Benchmarks
I'm benchmarking two tasks, how much time it takes to push `10_000` values and then to pop all of them:
```
test std_heap::push               ... bench:     101,009 ns/iter (+/- 1,465)
test std_heap::push_and_pop       ... bench:     669,717 ns/iter (+/- 124,892)
test my_binary_heap::push         ... bench:     104,930 ns/iter (+/- 7,285)
test my_binary_heap::push_and_pop ... bench:     459,216 ns/iter (+/- 19,489)
test kary_heap_2::push            ... bench:      93,337 ns/iter (+/- 841)
test kary_heap_2::push_and_pop    ... bench:     452,495 ns/iter (+/- 33,013)
test kary_heap_4::push            ... bench:      51,234 ns/iter (+/- 4,504)
test kary_heap_4::push_and_pop    ... bench:     377,595 ns/iter (+/- 31,432)
test kary_heap_8::push            ... bench:      32,694 ns/iter (+/- 3,230)
test kary_heap_8::push_and_pop    ... bench:     398,021 ns/iter (+/- 45,633)
test kary_heap_16::push           ... bench:      18,896 ns/iter (+/- 217)
test kary_heap_16::push_and_pop   ... bench:     569,050 ns/iter (+/- 5,304)
```