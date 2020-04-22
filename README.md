# Safe and Fast NIFs with Rust(ler)!

In this tiny dojo repository we'll be exposed to the creation of [Natively
Implemented Functions for the BEAM](http://erlang.org/doc/man/erl_nif.html)
using the [Rust programming language](https://www.rust-lang.org/) and the
[Rustler project](https://github.com/rusterlium/rustler).

The core premise here is that Rust, being a performant, reliable, and
productive language, is an excellent choice for building libraries that require
native support, for those use-cases where executing Erlang or Elixir code is
just not enough, or where a good Rust library is already available.

In particular, we will be creating a tiny module implementing a
dynamically-sized binary buffer that is:

* safe, and should never crash the BEAM, and
* fast!

## Prerequisites

To get started, please follow the installation guide from [Getting Started at
Rust-lang.org](https://www.rust-lang.org/learn/get-started). It should take a
couple of minutes, and the tooling is entirely self-contained. If you are on a
UNIX-like, you'll end up running this installer:

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

You will only be using `rustup` to manage the Rust toolchain, as the rest will
be handled via `mix`. Make sure you also have `mix`.

While knowledge about systems programming and type-systems is useful, we will be
limiting the actual Rust code to the smallest possible examples.


## Additional documentation

If you're interested in learning more about Rust, the [The Rust Programming
Language book](https://doc.rust-lang.org/stable/book/) is a fantastic
reference.
