## frontend webframework benchmark

```
test leptos_deep_creation                 ... bench:      80,455 ns/iter (+/- 28,291)
test leptos_deep_update                   ... bench:     395,647 ns/iter (+/- 88,409)
test leptos_fanning_out                   ... bench:     306,930 ns/iter (+/- 89,803)
test leptos_narrowing_down                ... bench:     202,961 ns/iter (+/- 31,444)
test leptos_narrowing_update              ... bench:     377,887 ns/iter (+/- 38,595)
test leptos_scope_creation_and_disposal   ... bench:     742,635 ns/iter (+/- 110,906)
test sycamore_deep_creation               ... bench:     278,049 ns/iter (+/- 20,804)
test sycamore_deep_update                 ... bench:     419,636 ns/iter (+/- 35,927)
test sycamore_fanning_out                 ... bench:     363,235 ns/iter (+/- 41,510)
test sycamore_narrowing_down              ... bench:     178,360 ns/iter (+/- 12,399)
test sycamore_narrowing_update            ... bench:     379,326 ns/iter (+/- 31,982)
test sycamore_scope_creation_and_disposal ... bench:     588,955 ns/iter (+/- 64,872)
```

```
test todomvc::leptos_todomvc_ssr             ... bench:       5,865 ns/iter (+/- 691)
test todomvc::leptos_todomvc_ssr_with_1000   ... bench:  23,014,535 ns/iter (+/- 3,427,326)
test todomvc::sycamore_todomvc_ssr           ... bench:      28,324 ns/iter (+/- 2,315)
test todomvc::sycamore_todomvc_ssr_with_1000 ... bench:  10,510,095 ns/iter (+/- 834,420)
test todomvc::tera::tera_todomvc             ... bench:       1,050 ns/iter (+/- 93)
test todomvc::tera::tera_todomvc_1000        ... bench:   1,249,643 ns/iter (+/- 71,902)
```


