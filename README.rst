RUST
===============

Install
---------

.. _Rust: https://www.rust-lang.org/tools/install

.. code-block:: bash

    # Install Rust toolchain
    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
    
    # Dependencies and tools: error: linker `cc` not found
    for Arch Linux: sudo pacman -S base-devel
    for Ubuntu: sudo apt install build-essential
    for Centos: sudo yum install gcc
    for Solus: sudo eopkg it -c system.devel

    # Update your system
    sudo apt update && sudo apt upgrade
    rustup update

    # Check the rust version
    rustc --version
    cargo --version
    


Hello World
-----------

1. Save main.rs

.. code-block:: bash

    // print a hello world in rust
    fn main() {
        println!("Hello, world!");
    }

2. Compile

.. code-block:: bash

    $ rustc main.rs

3. Run rust program in terminal

.. code-block:: bash

    $ ./main
    Hello, world!


Cargo Build
------------

.. code-block:: bash

    $ cargo new hello_world
    Created binary (application) `hello_world` package

    $ cd hello_world
    $ cargo run
    Hello, world!

    $ cargo build --release
    Compiling hello_world v0.1.0 (/home/mukesh/rust/hello_world)
    Finished release [optimized] target(s) in 0.29s

    $./target/release/hello_world
    Hello, world!