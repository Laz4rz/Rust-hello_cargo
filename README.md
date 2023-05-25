Cargo is a package manager for Rust. 
Cargo is a tool that allows Rust projects to declare their various dependencies and ensure that you’ll always get a repeatable build.

```
$ cargo --version
>> cargo 1.69.0 (6e9a83356 2023-04-12)
```

### Creating a package
```
$ cargo new hello_cargo
>> Created binary (application) `hello_cargo` package
```

Creating packages with cargo automatically setups:
- git repository
- configuration file (Cargo.toml)
- src directory with main.rs file

### Building a package
This package can be built by

```
$ cargo build
```

It will create an additional target folder which contains the executable and additional files. Executable can then be run with:

```
$ ./target/debug/hello_cargo
```

### Other
The package can be compiled and run at the same time by using

```
$ cargo run
```

Or just compiled, without creating the executable. This may be way faster for just checking whether the code compiles. 

```
$ cargo check
```

### Release build
Release build will make additional optimizations in the executable, but will probably take longer then the normal one. It will also create the executable in the target/release folder, instead of target/debug.

```
$ cargo build --release
```

### Cargo with git
Whenever cloning someones Rust repo it can be simply built with

```
$ git clone example.org/someproject
$ cd someproject
$ cargo build
```
