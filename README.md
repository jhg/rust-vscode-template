# {{project-name}}
Rust template for Cargo generate with VSCode extensions, tasks and GitHub actions.

![Crates.io version](https://img.shields.io/crates/v/{{project-name}}) ![Crates.io license](https://img.shields.io/crates/l/{{project-name}}) ![Crates.io downloads](https://img.shields.io/crates/d/{{project-name}})

## What does this template give you
- VSCode extension:
  - Use rust-analyzer and ignore RLS
  - LLDB debug extension
  - Test explorer
  - Crates search and versions check
  - Better TOML
  - TOML snippets
  - GitLens
  - ToDo tree
- VSCode tasks:
  - Cargo check, build & test
  - Rustup update
  - Cargo doc & doc --open
- GitHub actions:
  - Cargo audit daily, when push and in pull-request to main, master, dev or develop
  - Lint with Clippy and rustfmt when push and in pull-request
  - Cargo check & test weekly (maybe you want to remove this if you use Cargo.lock), when push and in pull-request
  - Cargo check & test with nightly daily
- Cargo.toml
  - Publish to false until you are ready to publish and change it

## Using this template
Install [`cargo-generate`](https://github.com/ashleygwilliams/cargo-generate) executing:
```
$ cargo install cargo-generate
```

Create a new crate using this template:
```
$ cargo generate --git https://github.com/jhg/rust-vscode-template.git --name myproject
```

## Get started
You need to [install Rust](https://www.rust-lang.org/tools/install) (recommended with rustup).

It's required, for Windows, to install [Visual Studio C++ Build tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/).

Also it's recommended to have installed [Git](https://git-scm.com/downloads) and
optionally [Visual Studio Code](https://code.visualstudio.com/?wt.mc_id=vscom_downloads).

If you use Visual Studio Code there are recommended extensions to add Rust support make things easy.

## Build
To build the crate run:
```
$ cargo build
```
If you're using Visual Studio Code and installed the recommended extensions you can use `ctrl+shift+b`/`⌘+shift+b`
(or menu `Terminal -> Run Build Task`) and run the task `Rust: cargo build`.

That will build with dev profile the crate at `target/debug/`.

## Tests
To run tests execute:
```
$ cargo test
```
If you're using Visual Studio Code you can use the menu `Terminal -> Run Task`
and run the task `Rust: cargo test`.

## Doc
To generate documentation run:
```
$ cargo doc --no-deps --document-private-items --all-features
```
Then open in your favorite browser `target/doc/{{crate_name}}/index.html` HTML document.

Also it has available a task `Rust: cargo doc` for Visual Studio Code.
But maybe you will prefer the task `Rust: cargo doc --open` to build and open the doc in the browser.
