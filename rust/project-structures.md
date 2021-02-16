# Creating a new Rust project
Running `cargo new` will create a new Rust project with the following scaffolding:

```
.
|- src/         # home of project code
|   |- main.rs
|- .gitignore   
|- Cargo.toml   # manifest a la package.json
```


main.rs created with this command includes the following dummy code:
```rust
fn main() {
    println!("Hello, world!");
}
```

- declare functions with `fn`
- `println!` is a **macro** to print to console. Macros are like "superfunctions", i.e. functions encapsulated to be presented in a more human-readable way
