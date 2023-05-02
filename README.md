## frontend webframework benchmarks

- leptos
- sycamore
- dioxus

### how to run

```bash
rustup default nightly
cargo bench
```

### benchmarks

- reactive

```text
test leptos_deep_creation                 ... bench:     110,208 ns/iter (+/- 21,354)
test leptos_deep_update                   ... bench:     407,354 ns/iter (+/- 103,459)
test leptos_fanning_out                   ... bench:     312,223 ns/iter (+/- 91,099)
test leptos_narrowing_down                ... bench:     204,127 ns/iter (+/- 22,674)
test leptos_narrowing_update              ... bench:     388,814 ns/iter (+/- 72,225)
test leptos_scope_creation_and_disposal   ... bench:     749,741 ns/iter (+/- 204,108)
test sycamore_deep_creation               ... bench:     285,691 ns/iter (+/- 50,319)
test sycamore_deep_update                 ... bench:     474,640 ns/iter (+/- 94,487)
test sycamore_fanning_out                 ... bench:     367,515 ns/iter (+/- 30,286)
test sycamore_narrowing_down              ... bench:     181,668 ns/iter (+/- 25,259)
test sycamore_narrowing_update            ... bench:     677,473 ns/iter (+/- 273,928)
test sycamore_scope_creation_and_disposal ... bench:     944,086 ns/iter (+/- 192,100)
```
- ssr

```text
test leptos_ssr_bench   ... bench:      13,994 ns/iter (+/- 3,748)
test sycamore_ssr_bench ... bench:      25,665 ns/iter (+/- 12,194)
test tera_ssr_bench     ... bench:       2,449 ns/iter (+/- 1,115)
```

- todomvc

```text
test todomvc::leptos_todomvc_ssr             ... bench:      12,843 ns/iter (+/- 5,691)
test todomvc::leptos_todomvc_ssr_with_1000   ... bench:  43,702,345 ns/iter (+/- 8,142,173)
test todomvc::sycamore_todomvc_ssr           ... bench:      52,757 ns/iter (+/- 20,625)
test todomvc::sycamore_todomvc_ssr_with_1000 ... bench:  38,442,436 ns/iter (+/- 18,403,507)
test todomvc::tera::tera_todomvc             ... bench:       2,205 ns/iter (+/- 999)
test todomvc::tera::tera_todomvc_1000        ... bench:   2,748,351 ns/iter (+/- 1,567,873)
```