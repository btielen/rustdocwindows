
## Error

Steps to reproduce on windows:

- `cargo build`
- `rustdoc src/some_docs.md --test --edition 2018 -L target/debug/deps` (same for edtion 2021)

results in error

`fatal error LNK1181: cannot open input file 'windows.lib'` error on windows.


```rust
extern crate tokio;

#[tokio::main]
async fn main() { }
```
