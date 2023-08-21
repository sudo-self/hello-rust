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
}
    

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
[Uploading Rust.rtf…](){\rtf1\ansi\ansicpg1252\cocoartf2709
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fmodern\fcharset0 CourierNewPSMT;\f1\fnil\fcharset0 Monaco;}
{\colortbl;\red255\green255\blue255;\red38\green255\blue255;\red255\green255\blue255;\red0\green0\blue0;
\red255\green255\blue255;\red113\green131\blue132;\red38\green147\blue135;\red34\green255\blue6;\red36\green255\blue255;
\red0\green0\blue0;\red255\green255\blue255;\red34\green255\blue6;\red251\green0\blue255;\red255\green255\blue255;
\red0\green0\blue0;\red114\green137\blue4;\red113\green130\blue132;\red113\green131\blue132;\red254\green255\blue10;
\red71\green91\blue98;\red33\green120\blue201;\red209\green27\blue35;\red38\green146\blue134;\red113\green131\blue132;
\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c8302\c100000\c100000;\cssrgb\c100000\c100000\c99985\c0;\cssrgb\c0\c1\c1;
\cssrgb\c100000\c100000\c100000\c0;\cssrgb\c51661\c58350\c58878;\cssrgb\c16698\c63502\c59872;\cssrgb\c0\c99725\c0;\cssrgb\c4983\c100000\c100000;
\cssrgb\c0\c1\c1;\cssrgb\c100000\c100000\c99971\c0;\cssrgb\c0\c100000\c0;\cssrgb\c100000\c7248\c100000;\cssrgb\c100000\c100000\c100000;
\cssrgb\c0\c0\c0;\cssrgb\c51735\c59494\c0;\cssrgb\c51518\c58195\c58852;\cssrgb\c51589\c58273\c58865;\cssrgb\c99555\c99475\c0;
\cssrgb\c34646\c43291\c45950;\cssrgb\c15379\c55095\c82900;\cssrgb\c86225\c19449\c18057;\cssrgb\c16585\c63320\c59740;\cssrgb\c51732\c58427\c58890;
\cssrgb\c0\c0\c0\c85000;}
\paperw11900\paperh16840\margl1440\margr1440\vieww26520\viewh19320\viewkind0
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\pardirnatural\partightenfactor0

\f0\fs36 \cf2 \cb3 \CocoaLigature0 INSTALL RUST ON MACos AND CREAT A NEW PROJECT\cf4 \cb5 \
\
\pard\pardeftab720\partightenfactor0
\cf4 \expnd0\expndtw0\kerning0
\CocoaLigature1 curl --proto \cf4 '=https'\cf4  --tlsv1.2 -sSf https://sh.rustup.rs | sh\
\
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\pardirnatural\partightenfactor0
\cf8 \kerning1\expnd0\expndtw0 \CocoaLigature0  stable-aarch64-apple-darwin installed\cf4 \
\
\
\cf9 \cb3 RELOAD SHELL TO INCLUDE CARGO\cf4 \cb5 \
\
source "$HOME/.cargo/env"\
\
\
\cf9 \cb3 START A NEW PROJECT \
\
\cf10 \cb11 Cargo new hello-rust\
\
\cf8 \cb5  Created binary (application) `hello-rust` package\
\
Cargo.toml = metadata\
\
Src/main.rs = application code\
\
\cf10 \cb3 cd hello-rust\cf8 \cb5 \
\
\cf10 \cb3 cargo run\
\cf12 \cb3 \
 Compiling hello-rust v0.1.0 (/Users/admin/hello-rust)\
    Finished dev [unoptimized + debuginfo] target(s) in 0.68s\
     Running `target/debug/hello-rust`\
\
\cf13 \cb11 Hello World!\cf12 \cb3 \
\cf10 \cb3 \
\
\cf8 \cb5 \
\cf9 \cb3 Adding Dependencies\cf8 \cb5 \
\
\pard\pardeftab720\sa600\partightenfactor0
\cf0 \cb14 \expnd0\expndtw0\kerning0
\CocoaLigature1 cargo add ferris-says@0.2\
\
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\pardirnatural\partightenfactor0
\cf8 \cb5 \kerning1\expnd0\expndtw0 \CocoaLigature0  Updating crates.io index\
      Adding ferris-says v0.2 to dependencies.\
             Features as of v0.2.0:\
             - clippy\
    Updating crates.io index\

\fs48 \cf4 \
\

\f1\fs36 \cf9 \cb3 Add the following line to \'93main.rs\'94\
\
\pard\pardeftab720\partightenfactor0

\f0 \cf4 \cb5 \expnd0\expndtw0\kerning0
\CocoaLigature1 use\cf4  ferris_says::say;\
\
\
Cargo build\
\
\
\
\
\pard\pardeftab720\partightenfactor0
\cf9 \cb3 Application written in main.rs\
\
\
\pard\pardeftab720\partightenfactor0
\cf19 \cb5 use\cf19  ferris_says::say; \cf19 // from the previous step\cf19 \
\cf19 use\cf19  std::io::\{stdout, BufWriter\};\
\
\cf19 fn\cf19  \cf19 main\cf19 () \{\
    \cf19 let\cf19  stdout = stdout();\
    \cf19 let\cf19  message = \cf19 String\cf19 ::from(\cf19 "Hello fellow Rustaceans!"\cf19 );\
    \cf19 let\cf19  width = message.chars().count();\
\
    \cf19 let\cf19  \cf19 mut\cf19  writer = BufWriter::new(stdout.lock());\
    say(message.as_bytes(), width, &\cf19 mut\cf19  writer).unwrap();\
\}\
    \cf19 \
\pard\pardeftab720\partightenfactor0
\cf9 \cb3 \
\pard\pardeftab720\partightenfactor0

\f1 \cf4 \cb5 \kerning1\expnd0\expndtw0 \CocoaLigature0 Cargo run \
\
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\pardirnatural\partightenfactor0
\cf8 > cargo run                                                                                                                     ~/hello-rust(main\uc0\u10007 )@JesseJesse.local\
   Compiling hello-rust v0.1.0 (/Users/admin/hello-rust)\
    Finished dev [unoptimized + debuginfo] target(s) in 0.56s\
     Running `target/debug/hello-rust`\
 __________________________\
< Hello fellow Rustaceans! >\
 --------------------------\
        \\\
         \\\
            _~^~^~_\
        \\) /  o o  \\ (/\
          '_   -   _'\
          / '-----' \\\
>                        \cf12 \cb25       \cf4 \cb5 \
\pard\pardeftab720\partightenfactor0

\fs20 \cf4 \
}


