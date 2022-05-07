# Rust to Python

This repository provides a mapping from Rust tooling and language features to Python.

# Tooling

| Tool | Rust | Python
| - | - | -
| Multi-version Installation | [rustup][rustup] | [pyenv][pyenv], [pyenv-win][pyenv-win]
| Package Repository | [crates.io][crates.io] | [PyPI][PyPI]
| Package Management | [Cargo][Cargo] | [Poetry][Poetry]
| Build Executables | [Cargo][Cargo] | [PyInstaller][PyInstaller]
| Code Formatting | [Rustfmt][Rustfmt] | [Black][Black], [isort][isort]
| Linting | [Clippy][Clippy] | [Flake8][Flake8]
| Unit Testing | [`#[test]`][test] | [pytest][pytest],
| Scripts | [cargo-script][cargo-script] | [Nox][Nox]

[rustup]: https://www.rust-lang.org/tools/install
[pyenv]: https://github.com/pyenv/pyenv
[pyenv-win]: https://github.com/pyenv-win/pyenv-win
[crates.io]: https://crates.io/
[PyPI]: https://pypi.org/
[Cargo]: https://doc.rust-lang.org/cargo/
[Poetry]: https://python-poetry.org/
[PyInstaller]: https://pyinstaller.org/en/stable/
[Rustfmt]: https://rust-lang.github.io/rustfmt
[Black]: https://black.readthedocs.io/en/stable/
[isort]: https://pycqa.github.io/isort/
[Clippy]: https://github.com/rust-lang/rust-clippy
[Flake8]: https://flake8.pycqa.org/en/latest/
[test]: https://doc.rust-lang.org/book/ch11-01-writing-tests.html
[pytest]: https://docs.pytest.org/
[cargo-script]: https://github.com/DanielKeep/cargo-script
[Nox]: https://nox.thea.codes/en/stable/
