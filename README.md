## Rust intro — quick notes (up to the Introduction)

Source video: https://www.youtube.com/watch?v=rQ_J9WH6CGk

### What Rust is

- A **systems programming language** aimed at performance comparable to C/C++.
- Designed to help write **reliable and efficient** programs.

### Why Rust is popular

- Focus on **memory safety** without needing a garbage collector.
- Helps prevent common bugs like:
    - null/dangling pointer issues
    - data races in concurrent code
    - use-after-free / double-free patterns (common in manual-memory languages)

### Core idea you’ll see throughout Rust

- Rust enforces safety mostly at **compile time** through strict rules.
- You’ll often hear about:
    - **ownership**
    - **borrowing**
    - **lifetimes**
- The goal: make invalid memory usage hard/impossible to compile.

### Where Rust is used

- Performance-critical tools and services
- CLI apps and developer tooling
- Backend services
- Embedded / low-level code (where control + safety matters)

### Key takeaways from this intro

- Rust is about balancing **speed + safety + modern language features**.
- The compiler is “strict” on purpose to catch bugs early.
- The rest of the course will build on ownership/borrowing concepts.

### Next

### Cargo (Rust’s build tool & package manager)

- **Cargo** is the default tool you use to create, build, run, and manage Rust projects.
- It helps with:
    - project scaffolding
    - dependency management (crates)
    - building & running
    - testing

#### Most common commands

- Create a new project:
    - `cargo new hello_rust`
- Go into the project folder:
    - `cd hello_rust`
- Build:
    - `cargo build`
    - (use `cargo build --release` for optimized builds)
- Run:
    - `cargo run`
- Check compile errors quickly (no binary output):
    - `cargo check`
- Run tests:
    - `cargo test`

#### Project structure (what you’ll usually see)

- `Cargo.toml` — project metadata + dependencies
- `src/main.rs` — main executable entry point (for binaries)
- `src/lib.rs` — library entry point (for libraries)

### Next

- Continue from where the video starts writing/running the first Rust program and explaining the project files (`Cargo.toml`, `src/main.rs`).
