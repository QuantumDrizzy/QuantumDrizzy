# Antonio Zambudio

> **Performance is a function of what you control. So I control all of it.**

**Research software engineer** building **bare-metal, high-performance systems** — and using them as
instruments to investigate hard problems. CUDA, Rust and C/C++ where latency and control decide the
outcome; Python where it pays. AI runs through it both ways: systems that *run* models, and systems
built *with* models (neural-guided annealers, compile-time-safe neural interfaces, forecasting
control loops). Solo, end to end, on bare metal (Arch Linux, CUDA-first) — with
**benchmarks anyone can re-run.** The hardware is a tool I command, not a limit: the skill is the
*architecture under the metal*, and it moves across whatever the silicon is — an edge board, a
single GPU, a cluster. *(NVIDIA by preference — CUDA, CUDA-Q, tensor cores, Blackwell.)*

**Systems first, always — but driven by research.** The fields below — quantum, neuroscience,
materials, energy — are proving grounds for the same skill, *not the identity*. Not a neuroscientist
or a materials physicist; the engineer who builds the systems to investigate them at the metal, and
who cares enough to get the physics right and the numbers honest. The through-line: *physics computes
by minimizing energy; the systems here exploit it.*

---

## Flagship — [Unibit](https://github.com/QuantumDrizzy/unibit): *what does this work actually cost the machine?*

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/unibit/master/docs/img/density.png" width="760">
</p>

A 256-bit instruction set, a cycle-accurate emulator, an assembler and an object format — written in
Rust with **zero dependencies** — built to answer one question honestly: how many instructions must an
architecture retire to do real work?

Three workloads measured: int8 matvec at a 7B model's hidden size, Ising coupling energy, a 256-site
MPS contraction. The headline result is a **negative** one — `VDOT.B` has exactly the same arithmetic
density as AVX2's `VPMADDUBSW`, so 256-bit width buys nothing; only the fused `ZIPPER2` contraction is
genuinely ahead. Measurement also exposed a hole in my own design (no mixed-width int8×int64 dot,
costing 34 % of achievable density), documented rather than hidden.

**And the number I did not publish:** dividing instruction counts by an assumed 3 GHz would have shown
this beating both CPU and GPU. The host baselines are ~97 % dispatch overhead — an *empty* CUDA matmul
costs 45.66 µs against 46.8 µs measured — so that comparison measures Python, not silicon. Start here
if you want to know how I treat a number that flatters me.

---

## Research grounds — the same skill, pointed at hard problems

**[DRIFT](https://github.com/QuantumDrizzy/DRIFT) — the structure under the problem.**
Optimization, self-assembly and neural memory (Hopfield) read as ground states of *one* Ising
Hamiltonian — the unification thesis, made measurable and benchmarked against the Landauer floor of
computation.

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/DRIFT/master/figures/phase7_roofline.png" width="720">
</p>

How far is real hardware from the physical floor of computation? **Six orders of magnitude above the
Landauer wall** — DDR5 and GPU arithmetic on one side, DNA polymerase and the Margolus–Levitin bound on
the other. That gap is the headroom unconventional substrates are competing for.

**[SUBSTRATE](https://github.com/QuantumDrizzy/SUBSTRATE) — can I make the metal go fast, and prove it?**
Multi-physics simulation engine. The physics is the hard problem; the point is the engine underneath:
**hand-written CUDA (sm_120) with an honest, kernel-only roofline — 3× → 139× vs JAX-CPU across
lattice sizes, end-to-end break-even stated, not hidden** — plus tensor-network solvers for many-body
systems.

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/SUBSTRATE/master/docs/showcase/galaxy-rotation-dark-matter.png" width="760">
</p>

**[AETHER](https://github.com/QuantumDrizzy/AETHER) — hard physics, implemented *correctly*.**
Computational-materials lab: electronic structure, the full topological set (SSH, Haldane, Kane–Mele),
metamaterials, GPU solvers with measured speedups, inverse design. **~90 tests; every claim checked
against a closed form.** Correctness isn't optional.

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/AETHER/master/figures/ising2d_gpu_speedup.png" width="680">
</p>

The benchmark publishes where CUDA **loses**: 0.3× at 32², break-even near L≈100, 222× at 1024². A
speedup curve that never dips below 1× is a curve with the small sizes quietly removed.

**[Blaze](https://github.com/QuantumDrizzy/Blaze) — the method that makes the rest tractable.**
Tensor-Train / MPS compression for high-order scientific and quantum-state data: GPU SVD over a C ABI
to Rust, MPS-to-circuit bridge, int8 quantisation with **measured** fidelity. Bond dimension χ is the
accuracy-against-cost dial the other repositories turn — the numerical method underneath the physics,
not a side project.

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/Blaze/master/docs/img/fidelity_matrix_qpt.png" width="640">
</p>

