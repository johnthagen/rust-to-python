# Rust to Python

This repository provides a mapping from Rust tooling and language features to Python.

# Tooling

| Tool | Rust | Python
| - | - | -
| Multi-version Installation | [rustup][rustup] | [pyenv][pyenv], [pyenv-win][pyenv-win]
| Package Repository | [crates.io][crates.io] | [PyPI][PyPI]
| Package Management | [Cargo][Cargo] | [Poetry][Poetry]
| Build Executables | [Cargo][Cargo] | [PyInstaller][PyInstaller]
| Type Checking | [Cargo][Cargo] | [Mypy]
| Code Formatting | [Rustfmt][Rustfmt] | [Black][Black], [isort][isort]
| Linting | [Clippy][Clippy] | [Flake8][Flake8]
| Unit Testing | [`#[test]`][test] | [pytest][pytest]
| Scripts | [cargo-script][cargo-script] | [Nox][Nox]

[rustup]: https://www.rust-lang.org/tools/install
[pyenv]: https://github.com/pyenv/pyenv
[pyenv-win]: https://github.com/pyenv-win/pyenv-win
[crates.io]: https://crates.io/
[PyPI]: https://pypi.org/
[Cargo]: https://doc.rust-lang.org/cargo/
[Poetry]: https://python-poetry.org/
[PyInstaller]: https://pyinstaller.org/en/stable/
[Mypy]: https://mypy.readthedocs.io/en/stable/
[Rustfmt]: https://rust-lang.github.io/rustfmt
[Black]: https://black.readthedocs.io/en/stable/
[isort]: https://pycqa.github.io/isort/
[Clippy]: https://github.com/rust-lang/rust-clippy
[Flake8]: https://flake8.pycqa.org/en/latest/
[test]: https://doc.rust-lang.org/book/ch11-01-writing-tests.html
[pytest]: https://docs.pytest.org/
[cargo-script]: https://github.com/DanielKeep/cargo-script
[Nox]: https://nox.thea.codes/en/stable/

# Environments

| Environment | Rust | Python
| - | - | -
| WASM | [wasm-pack][wasm-pack] | [PyScript][PyScript], [Pyodide][Pyodide], [CPython WASM][CPython WASM]
| Embedded | [Embedded Rust][Embedded Rust] | [MicroPython][MicroPython], [CircuitPython][CircuitPython]

[wasm-pack]: https://rustwasm.github.io/
[PyScript]: https://pyscript.net/
[Pyodide]: https://pyodide.org/en/stable/
[CPython WASM]: https://github.com/ethanhs/python-wasm
[Embedded Rust]: https://docs.rust-embedded.org/book/
[MicroPython]: https://micropython.org/
[CircuitPython]: https://circuitpython.org/

# Language Features

| Feature | Rust | Python
| - | - | -
| Interface | [`trait`][trait] | [`Protocol`][Protocol]
| Generics | [`<T>`][Rust Generic] | [`Generic`][Generic]
| Algebraic Data Type | [`enum`][enum] | [`Enum`][Enum], [`Union` of `dataclass`][union-dataclass]
| Fixed-sized Numerics | `u8`, `u16`, etc. | [NumPy Data Types][NumPy Data Types]
| Foreign Function Interface | [FFI][Rust FFI] | [CFFI][CFFI]

[trait]: https://doc.rust-lang.org/book/ch10-02-traits.html
[Protocol]: https://docs.python.org/3/library/typing.html#typing.Protocol
[Rust Generic]: https://doc.rust-lang.org/book/ch10-01-syntax.html
[Generic]: https://docs.python.org/3/library/typing.html#typing.Generic
[enum]: https://doc.rust-lang.org/book/ch06-01-defining-an-enum.html
[Enum]: https://docs.python.org/3/library/enum.html
[union-dataclass]: https://stackoverflow.com/a/71519690
[NumPy Data Types]: https://numpy.org/doc/stable/user/basics.types.html
[Rust FFI]: https://doc.rust-lang.org/nomicon/ffi.html
[CFFI]: https://cffi.readthedocs.io/en/latest/

# Rust/Python Interop

- [PyO3](https://pyo3.rs/)
