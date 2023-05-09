# bazel-broken-dep

Build dependency crate feature propagation is broken with `rules_rust` >= 0.17.x.

```
# Fails because of broken crate feature propagation
$ bazel test //...
```

```
# Works
$ cargo test
```
