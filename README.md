# binaries

This repository precompiles binaries and caches them in GitHub Releases for CI
jobs of the [@stellar] GitHub org.

[@stellar]: https://github.com/stellar

## Usage

**Use of the binaries stored here are not recommended for general purpose use.
They're only intended for use supporting the [@stellar] CI jobs.**

Add the following to a workflow to install a binary here. The version must be
specified as a tag, as the tag also identifies which release to download the
binaries from.

```yml
- uses: stellar/binaries@v10
  with:
    name: cargo-set-rust-version
    version: 0.5.0
```
