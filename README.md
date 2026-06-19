# Antonio Zambudio

> **Performance is a function of what you control. So I control all of it.**

**I build bare-metal, high-performance systems** — the fast, low-level code under
hard problems. CUDA, Rust and C/C++ where latency and control decide the outcome;
Python where it pays. Solo, end to end, on my own hardware (RTX 5060 Ti / Blackwell
sm_120, Arch Linux) — with **benchmarks anyone can re-run.**

I'm a performance/systems engineer first. The domains below — quantum, neuroscience,
materials, energy — are just where I point the same skill. The through-line:
*physics computes by minimizing energy; I write the systems that exploit it, at the metal.*

**Stack:** CUDA (hand-written kernels, sm_120 roofline) · Rust (control loops, systems) ·
C / C++17 (compile-time guarantees) · Python (ML, glue, analysis). No cloud, by choice.

---

## Flagship — [SUBSTRATE](https://github.com/QuantumDrizzy/SUBSTRATE): *can I make the metal go fast — and prove it?*

A multi-physics / bio-electromagnetics simulation engine. The physics is the hard problem;
the point is the engine underneath: **hand-written CUDA (sm_120) with an honest,
kernel-only roofline — 3×→154× vs JAX-CPU, end-to-end break-even stated, not hidden** —
plus tensor-network solvers for many-body systems. Start here if you want to know
whether I can write fast kernels and back the numbers.

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/SUBSTRATE/master/benchmarks/plots/plaquette_roofline.png" width="720">
</p>

---

## Selected systems — each proves one thing

**[BLACKWALL](https://github.com/QuantumDrizzy/BLACKWALL) · [ICEPICK](https://github.com/QuantumDrizzy/ICEPICK) · [FLATLINE](https://github.com/QuantumDrizzy/FLATLINE) — I reverse-engineer the silicon I run on.**
A three-part Blackwell (sm_120) teardown, hand-written CUDA: the compute roofline
(BLACKWALL), the microarchitecture beneath it — instruction latencies, caches, the SASS the
compiler actually emits (ICEPICK), and the energy/thermal wall (FLATLINE). The metal,
measured directly — compute · communication · energy.

**[AETHER](https://github.com/QuantumDrizzy/AETHER) — I implement hard physics *correctly*.**
Computational-materials lab: electronic structure, the full topological set (SSH, Haldane,
Kane–Mele), metamaterials, GPU-accelerated solvers, inverse design. **~90 tests; every claim
checked against a closed form.** Correctness isn't optional.

**[KHAOS](https://github.com/QuantumDrizzy/KHAOS) — I build real-time systems where safety is *enforced*, not hoped for.**
Closed-loop BCI kernel: a CUDA DSP hot-path, stimulation limits guaranteed by the C++
compiler (`static_assert`), three independent safety layers, post-quantum audit ledger.
Sub-100 µs is the design target — *marked unverified until benchmarked end-to-end.*

**[HELIOS](https://github.com/QuantumDrizzy/HELIOS) — I build control loops that can't go down.**
24/7 predictive DC-microgrid controller. Rust MPPT loop (100 ms tick), CNN-LSTM forecasting,
post-quantum trust anchors. Where the lights actually have to stay on.

**[DRIFT](https://github.com/QuantumDrizzy/DRIFT) — I see the structure under the problem.**
Optimization, self-assembly and neural memory (Hopfield) read as ground states of *one*
Ising Hamiltonian — the unification thesis, made measurable and benchmarked against the
Landauer floor of computation.

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/DRIFT/master/figures/phase7_four_faces.png" width="720">
</p>

**[Blaze](https://github.com/QuantumDrizzy/Blaze) — I compress massive scientific & quantum data on the GPU.**
Tensor-Train / MPS compression, GPU SVD, MPS↔circuit bridge. The specialist tool the rest
of the ecosystem leans on.

---

*More in the repos — same spine, other proving grounds. Everything is mine, on my own
hardware, reproducible.*
