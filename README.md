# byteview

Fast line/byte counter written in Rust

Small but I use it weekly.

## Highlights

- Parallel over files with std threads
- Zero dependencies outside std
- Reads stdin or multiple files
- Counts lines, words and bytes like wc

## Examples

```bash
./target/release/byteview src/*.rs
cat README.md | ./target/release/byteview
```

## Installation

```bash
cargo build --release
```

## Project structure

```text
├── .github/
│   ├── dependabot.yml
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── Cargo.toml
├── LICENSE
└── Makefile
```

## Development

```bash
cargo test
cargo clippy -- -D warnings
```
