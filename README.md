# Antonio Zambudio

> **Performance is a function of what you control. So I control all of it.**

Research Software Engineer / Systems Architect. I build bare-metal,
high-performance systems end to end — Rust, C, C++ and CUDA where latency and
control matter; Python where it pays. My own stack, on my own hardware (RTX 5060
Ti / Blackwell sm_120, Arch Linux), with benchmarks I can defend.

The work spans five domains, with one thread running through all of them:
**physics computes by minimizing energy — I build the systems that exploit it.**

## Five domains, one stack

- **AI** — agentic architectures, low-latency inference, distributed training
- **Quantum** — tensor networks, ground-state methods, quantum-inspired optimization
- **Computational neuroscience** — closed-loop BCI, attractor dynamics, energy-minimization models
- **Materials & condensed matter** — electronic structure, topological phases, metamaterials, unconventional computing substrates
- **Energy / solar** — predictive DC-microgrid control, post-quantum trust anchors

The brain, the crystal, the optimizer, the controller — same physics, all
relaxing to a minimum. Bare metal is the only honest place to do that.

## The pillars

Five domain bets, each a real system with code, tests and defensible numbers:

### [HELIOS](https://github.com/QuantumDrizzy/HELIOS) — *AI × energy*
24/7 predictive DC-microgrid controller. Rust MPPT control loop, CNN-LSTM
generation forecasting, post-quantum trust anchors. *Where the lights actually
have to stay on.*

### [KHAOS](https://github.com/QuantumDrizzy/KHAOS) — *AI × neuroscience*
Closed-loop BCI kernel: CUDA DSP pipeline designed for sub-millisecond latency,
neuroethics enforced at compile time (`static_assert` stimulation limits), and a
post-quantum-secured audit ledger. Three independent safety layers; validated in
simulation today.

### [SUBSTRATE](https://github.com/QuantumDrizzy/SUBSTRATE) — *AI × quantum*
Multi-scale physics & quantum-biology simulation. Hand-written CUDA (sm_120) with
an honest **kernel-only roofline (3×→154× vs JAX-CPU)** and tensor-network solvers
for cryptochrome spin dynamics, EM fields, and many-body systems.

### [AETHER](https://github.com/QuantumDrizzy/AETHER) — *AI × materials*
Computational-materials lab: tight-binding electronic structure (graphene, hBN,
and the full topological set — SSH winding, Haldane Chern, Kane–Mele Z₂),
metamaterials (auxetic mechanical + photonic band gaps), reservoir computing,
simulated annealing, and self-organisation (active matter, reaction–diffusion,
cellular automata). ~90 validation tests; every claim checked against a closed
form or a reference.

### [Blaze](https://github.com/QuantumDrizzy/Blaze) — *the compressor*
Tensor-Train / MPS compression for high-order scientific and quantum-state data.
GPU SVD, MPS↔circuit bridge, quantization. Cross-cuts the ecosystem; also the χ
compute-density thermometer in [DRIFT](https://github.com/QuantumDrizzy/DRIFT).

---

## A glimpse of the work

[DRIFT](https://github.com/QuantumDrizzy/DRIFT) reads optimization, self-assembly,
self-replication, and neural memory (Hopfield, Nobel Physics 2024) as **ground
states of one Ising Hamiltonian** — the unification thesis, made measurable:

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/DRIFT/master/figures/phase7_four_faces.png" alt="DRIFT — four faces, one engine" width="720">
</p>

How far is real hardware from the physical floor of computation? **Six orders of
magnitude above the Landauer wall** — that gap is the headroom for unconventional
computing substrates:

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/DRIFT/master/figures/phase7_roofline.png" alt="cosmic roofline — real hardware vs. Landauer floor" width="720">
</p>

In **[AETHER](https://github.com/QuantumDrizzy/AETHER)**, the same edge-of-chaos
shows up as a topological phase diagram — complex hopping opens lobes of non-zero
Chern number (a quantum anomalous Hall insulator), matched to the analytic boundary:

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/AETHER/master/figures/haldane_phase_diagram.png" alt="AETHER — Haldane topological phase diagram" width="640">
</p>

In **[SUBSTRATE](https://github.com/QuantumDrizzy/SUBSTRATE)**, the performance
story is told honestly — a kernel-only roofline against the computed hardware peak:

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/SUBSTRATE/master/benchmarks/plots/plaquette_roofline.png" alt="SUBSTRATE — kernel roofline" width="640">
</p>

And **[Blaze](https://github.com/QuantumDrizzy/Blaze)** quantifies the price of
compression — truncation error against retained rank for entangled states:

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/Blaze/master/docs/img/error_vs_rank.png" alt="Blaze — compression error vs rank" width="640">
</p>

---

## Other open & active work

- **[DRIFT](https://github.com/QuantumDrizzy/DRIFT)** — A microscope for physical
  computation. Four faces, one Ising engine; tensor-network χ as the compute-density
  thermometer; reservoir capacity at the edge of chaos.
- **[NIGHTWATCH](https://github.com/QuantumDrizzy/NIGHTWATCH)** — Real-time
  wide-field IR detection & tracking. CUDA CA-CFAR detection + Kalman tracking +
  TensorRT INT8 classification, with TLE catalogue cross-matching for overhead
  objects.

Several larger systems are in private development and can be discussed directly.

---

## Stack

**Systems / bare-metal** — Rust · C · C++ · CUDA (sm_120 Blackwell) · CUDA-Q · Assembly · `no_std` hot paths

**GPU / HPC** — cuBLAS · cuBLASLt · TensorRT · Flash Attention · NCCL · SLURM · Nsight profiling · roofline analysis

**Quantum / tensor networks** — Cirq · TT / MPS / TEBD / DMRG · QUBO / Ising · Lanczos / Krylov · simulated & quantum annealing

**Physics & simulation** — FDTD (Yee + PML) · tight-binding & band structure · topological invariants (Chern / Z₂ / winding) · reservoir computing · reaction–diffusion · Monte-Carlo & criticality · thermodynamics of computation (Landauer)

**AI / ML** — Python · PyTorch · CNN-LSTM · GNNs · NumPy / SciPy · ridge / spectral methods

**Security & correctness** — post-quantum primitives (ML-KEM / ML-DSA) · compile-time safety (`static_assert`) · SHA-3 audit ledgers · auditable, test-backed code

**Infra** — Arch Linux · bare-metal · local-first · no cloud by default

---

*Bare-metal · local-first · honest benchmarks · no cloud by default.*
