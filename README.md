# simple_logger [![](https://img.shields.io/github/tag/borntyping/rust-simple_logger.svg)](https://github.com/borntyping/rust-simple_logger/tags) [![](https://img.shields.io/travis/borntyping/rust-simple_logger.svg)](https://travis-ci.org/borntyping/rust-simple_logger) [![](https://img.shields.io/github/issues/borntyping/rust-simple_logger.svg)](https://github.com/borntyping/rust-simple_logger/issues)

A logger that prints all messages with a readable output format.

The output format is based on the format used by [Supervisord](http://supervisord.org/).

* [Source on GitHub](https://github.com/borntyping/rust-simple_logger)
* [Packages on Crates.io](https://crates.io/crates/simple_logger)
* [Builds on Travis CI](https://travis-ci.org/borntyping/rust-simple_logger)

Usage
-----

```rust
#[macro_use]
extern crate log;
extern crate simple_logger;

fn main() {
    simple_logger::init().unwrap();

    warn!("This is an example message.");
}
```

This outputs:

```
2015-02-24 01:05:20 WARN [logging_example] This is an example message.
```

You can run the above example with:

```bash
cargo run --example init
```

Licence
-------

`simple_logger` is licenced under the [MIT Licence](http://opensource.org/licenses/MIT).

Authors
-------

Written by [Sam Clements](sam@borntyping.co.uk).
