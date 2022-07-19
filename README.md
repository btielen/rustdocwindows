# Rustdoc bug on windows

Steps to reproduce on windows

- `git clone https://github.com/btielen/rustdocwindows.git`
- `cd rustdocwindows`
- `cargo build`
- `rustdoc src/some_docs.md --test --edition 2018 -L target/debug/deps`

results in error

`  = note: LINK : fatal error LNK1181: cannot open input file 'windows.lib'`


## Environment

- Windows 10
- stable-x86_64-pc-windows-msvc (default)
- rustdoc 1.62.0 (a8314ef7d 2022-06-27)
- rustc 1.62.0 (a8314ef7d 2022-06-27)