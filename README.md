Cargo is a package manager for Rust. 
Cargo is a tool that allows Rust projects to declare their various dependencies and ensure that you’ll always get a repeatable build.

```
cargo --version
>> cargo 1.69.0 (6e9a83356 2023-04-12)
```

```
cargo new hello_cargo
>> Created binary (application) `hello_cargo` package
```

Creating packages with cargo automatically setups:
- git repository
- configuration file (Cargo.toml)
- src directory with main.rs file
