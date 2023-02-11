# rust_no_std_hello_world
 embedded dev


prereqs
```
- Linux
```



```bash
rustup default nightly
rustup update
rustc --version --verbose
rustup component add rust-src --toolchain nightly-x86_64-unknown-linux-gnu
cargo +nightly rustc -- --version
cargo +nightly run -Zbuild-std=core,alloc --target x86_64-unknown-linux-gnu
# cargo +nightly build -Zbuild-std=core,alloc --target x86_64-unknown-linux-gnu
# cargo +nightly build -Zbuild-std=core,alloc --release --target x86_64-unknown-linux-gnu
```



target arch can be switched to:
```
https://docs.rust-embedded.org/embedonomicon/compiler-support.html#built-in-target
```