# mandelbrot-py

Demo for Rust/Python integration

## Run Rust-only version

```
cargo build --release
./target/release/mandelbrot image.png
```

## Run via Python interface

```
python3 -mvenv .
bin/pip install -e .
./bin/mandelbrot_py image.png
```

## Directory contents

src/mandelbrot.rs
    Rust lib which does the actual computation

src/main.rs
    Rust command line wrapper

src/lib.rs
    Python bindings

mandelbrot/__init__.py
    Python command line wrapper
