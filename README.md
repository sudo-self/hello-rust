# hello-rust
### INSTALL RUST ON MACos AND CREAT A NEW PROJECT

curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

 stable-aarch64-apple-darwin installed


### RELOAD SHELL TO INCLUDE CARGO

source "$HOME/.cargo/env"


### START A NEW PROJECT 

Cargo new hello-rust

 Created binary (application) `hello-rust` package

Cargo.toml = metadata

Src/main.rs = application code

cd hello-rust

cargo run
Compiling hello-rust v0.1.0 (/Users/admin/hello-rust)
    Finished dev [unoptimized + debuginfo] target(s) in 0.68s
     Running `target/debug/hello-rust`

Hello World!



### Adding Dependencies

cargo add ferris-says@0.2

 Updating crates.io index
      Adding ferris-says v0.2 to dependencies.
             Features as of v0.2.0:
             - clippy
    Updating crates.io index


### Add the following line to “main.rs”

use ferris_says::say;


Cargo build




### Application written in main.rs


use ferris_says::say; // from the previous step
use std::io::{stdout, BufWriter};

fn main() {
    let stdout = stdout();
    let message = String::from("Hello fellow Rustaceans!");
    let width = message.chars().count();

    let mut writer = BufWriter::new(stdout.lock());
    say(message.as_bytes(), width, &mut writer).unwrap();

    

Cargo run 

> cargo run                                                                                                                     ~/hello-rust(main✗)@JesseJesse.local
   Compiling hello-rust v0.1.0 (/Users/admin/hello-rust)
    Finished dev [unoptimized + debuginfo] target(s) in 0.56s
     Running `target/debug/hello-rust`
 __________________________
< Hello fellow Rustaceans! >
 --------------------------
        \
         \
            _~^~^~_
        \) /  o o  \ (/
          '_   -   _'
          / '-----' \
>                              

![Screenshot 2023-08-21 at 12 45 53 AM](https://github.com/sudo-self/hello-rust/assets/119916323/4a8def80-16e1-46ed-969f-1182d347426b)
