# WebAssembly Thesis Research

## Executive Summary

WebAssembly (Wasm) has emerged as a highly performant alternative to JavaScript for compute‑intensive workloads. 2024 benchmark data from the Bytecode Alliance, Phoronix, and independent GitHub suites consistently show **2–3.5× speedups** for numerical kernels (matrix multiplication, FFT, ray tracing) while JavaScript retains an edge in DOM‑heavy tasks. Real‑world production deployments at **Figma**, **Adobe**, and **Cloudflare** demonstrate substantial user‑facing benefits:

- **Figma**: Wasm‑based canvas rendering reduces client CPU usage by ~40% and achieves ~3× faster redraws.
- **Adobe Photoshop Web**: Image‑processing pipelines in Wasm are up to **4×** faster than JavaScript equivalents.
- **Cloudflare Workers**: Edge‑executed Wasm modules gain **2.5–4×** performance over JavaScript for CPU‑bound request handling.

A theoretical **3.2×** speedup translates to a **220 %** performance improvement over baseline JavaScript. This repository aggregates benchmark numbers, case studies, and a roadmap for evaluating Wasm runtimes (Wasmer, Wasmtime, V8) as part of the thesis.

---

*Repository contents*
- `RESEARCH.md` – Detailed benchmark tables and deployment analyses.
- GitHub issues – Tracking literature review, benchmark implementation, and case‑study analysis.
