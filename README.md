# {{project-name}}
Rust template for Cargo generate with VSCode extensions and tasks.

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
If you're using Visual Studio Code and installed the recommended extensions you can use `ctrl+shift+b`
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
