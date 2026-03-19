# WebAssembly Fundamentals & AssemblyScript Overview

## WebAssembly (Wasm)
- **Binary instruction format** designed as a portable compilation target for high‑level languages on the web.
- Executes in a sandboxed environment with near‑native performance.
- Core features: linear memory, tables, multi‑value returns, SIMD, and Garbage Collection (GC) proposals (official as of 2024).
- Runtimes: browsers (V8, SpiderMonkey, JavaScriptCore) and standalone engines (Wasmer, Wasmtime, WasmEdge).
- Use‑cases: compute‑heavy algorithms, game engines, image processing, cryptography, and edge‑computing.

## AssemblyScript
- **What it is**: A TypeScript‑like language that compiles directly to Wasm.
- **Key traits**:
  - Statically typed subset of TypeScript; no runtime objects.
  - Generates compact Wasm binaries (10‑50 KB typical).
  - Supports SIMD, bulk‑memory, and WasmGC as of v0.27 (2024).
  - Integrates with npm; CLI `asc` produces `.wasm` and JavaScript glue code.
- **Performance**: Benchmarks (as‑benchmark suite 2024) show AssemblyScript Wasm modules achieving 2‑3× speedups over pure JavaScript for numeric kernels.
- **Ecosystem**: NPM package `@assemblyscript/loader`, VS Code extension, tutorials, and growing community of game‑dev and crypto libraries.

## Relevance to Thesis
Understanding Wasm's runtime characteristics and the tooling around AssemblyScript provides a baseline for evaluating runtime performance optimizations across Wasmer, Wasmtime, and V8.
