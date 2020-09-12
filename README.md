# rustynetes
An attempt at a Kubernetes like container orchestrator written in Rust.

**_DISCLAIMER: I have no idea what I'm doing and this probably won't work. This is a just for fun project and is not intended for use in production._**

## Requirements
Since this uses rocket as the API server, we currently require a **nightly** rustc. We recommend you use [rustup](https://rustup.rs/) to install or configure such a version.
```
rustup override set nightly
```

## Developing
To iterate quickly, we use `watchexec` to continuously run `cargo run` any time a .rs file is changed:
```
cargo install watchexec
```
or
```
brew install watchexec
```
then
```
watchexec --exts rs --restart "cargo run"
```

