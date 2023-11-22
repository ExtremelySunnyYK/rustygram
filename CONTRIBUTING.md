# Contributing

Before contributing, please read [our code style](https://github.com/ExtremelySunnyYK/rustygram/blob/master/CODE_STYLE.md) and [the license](https://github.com/ExtremelySunnyYK/rustygram/blob/master/LICENSE).

To change the source code, fork the `master` branch of this repository and work inside your own branch. Then send us a PR into `master` branch and wait for the CI to check everything. However, you'd better check changes first locally:

```
cargo clippy --all --all-features --all-targets
cargo test --all
RUSTDOCFLAGS="--cfg docsrs" cargo doc --open --all-features
# Using nightly rustfmt
cargo +nightly fmt --all -- --check
```

To report a bug, suggest new functionality, or ask a question, go to [Issues](https://github.com/ExtremelySunnyYK/rustygram/issues). Try to make MRE (**M**inimal **R**eproducible **E**xample) and specify your teloxide version to let others help you.
