# bazel-broken-dep

Build dependency crate feature propagation is broken with `rules_rust` > 0.20.0.

```
# Fails because of broken crate feature propagation
$ bazel test //...
```

```
# Works
$ cargo test
```
