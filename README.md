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
| Upgrade to New Language Features | [`cargo fix`][cargo-fix] | [`pyupgrade`][pyupgrade]

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
[cargo-fix]: https://github.com/rust-lang/rustfix
[pyupgrade]: https://github.com/asottile/pyupgrade

> For a Python project example that incorporates these tools, see 
> [python-blueprint](https://github.com/johnthagen/python-blueprint).

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
| Generics | [`<T>`][Rust Generic] | [`list[T]` etc.][PEP 585], [`TypeVar`][TypeVar], [`Generic`][Generic]
| Pattern Matching | [`match`][Pattern Syntax] | [`match`][PEP 634]
| Anonymous Function | [`\|x\| { x + 1 }`][Closure] | [`lambda x: x + 1`][Lambda]
| Foreign Function Interface | [FFI][Rust FFI] | [CFFI][CFFI]

[trait]: https://doc.rust-lang.org/book/ch10-02-traits.html
[Protocol]: https://docs.python.org/3/library/typing.html#typing.Protocol
[Rust Generic]: https://doc.rust-lang.org/book/ch10-01-syntax.html
[PEP 585]: https://peps.python.org/pep-0585/
[TypeVar]: https://docs.python.org/3/library/typing.html#generics
[Generic]: https://docs.python.org/3/library/typing.html#typing.Generic
[Pattern Syntax]: https://doc.rust-lang.org/book/ch18-03-pattern-syntax.html
[PEP 634]: https://peps.python.org/pep-0634/
[Closure]: https://doc.rust-lang.org/book/ch13-01-closures.html
[Lambda]: https://docs.python.org/3/reference/expressions.html#lambda
[Rust FFI]: https://doc.rust-lang.org/nomicon/ffi.html
[CFFI]: https://cffi.readthedocs.io/en/latest/

# Data Structures

| Data Structure | Rust | Python
| - | - | -
| Data Type | [`struct`][struct] | [`@dataclass`][dataclass]
| Algebraic Data Type | [`enum`][enum] | [`Enum`][Enum], [`Union` of `dataclass`][union-dataclass]
| Result | [`Result`][Result] | [`returns.Result`][returns Result]
| Optional | [`Option`][Option] | [`T \| None`][Optional], [`returns.Maybe`][Maybe]
| Fixed-sized Numerics | [`u8`, `u16`, etc.][Rust Data Types] | [NumPy Data Types][NumPy Data Types]

[struct]: https://doc.rust-lang.org/book/ch05-01-defining-structs.html
[dataclass]: https://docs.python.org/3/library/dataclasses.html
[enum]: https://doc.rust-lang.org/book/ch06-01-defining-an-enum.html
[Enum]: https://docs.python.org/3/library/enum.html
[union-dataclass]: https://stackoverflow.com/a/71519690
[Result]: https://doc.rust-lang.org/std/result/
[returns Result]: https://returns.readthedocs.io/en/latest/pages/result.html
[Option]: https://doc.rust-lang.org/std/option/
[Optional]: https://docs.python.org/3/library/typing.html#typing.Optional
[Maybe]: https://returns.readthedocs.io/en/latest/pages/maybe.html
[Rust Data Types]: https://doc.rust-lang.org/book/ch03-02-data-types.html
[NumPy Data Types]: https://numpy.org/doc/stable/user/basics.types.html

# Rust/Python Interop

- [PyO3](https://pyo3.rs/)

# Misc Rust and Python Similarities

- Both languages prefer `snake_case` naming over `lowerCamelCase`
- Both languages use suffix type syntax (e.g. `x: int` / `x: i32`)
- Neither language is controlled by a single company
