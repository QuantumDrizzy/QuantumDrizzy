# Antonio Zambudio

> **Performance is a function of what you control. So I control all of it.**

Research Software Engineer / Systems Architect. Bare-metal systems work — Rust, C, C++, CUDA where it matters; Python where it pays. I build my own stack, on my own hardware, with benchmarks I can defend.

The work spans four frontiers, with one thread running through them: **physics computes by minimizing energy. I build the systems that exploit it.**

## Four frontiers, one stack

- **AI** — agentic architectures, low-latency inference, distributed training
- **Quantum** — tensor networks, ground-state methods, quantum-inspired optimization
- **Computational neuroscience** — closed-loop BCI, attractor dynamics, energy-minimization models
- **Energy / solar** — sovereign DC-microgrid control, post-quantum trust anchors

The brain, the crystal, the optimizer, the controller — same physics, all relaxing to a minimum. The hardware is the only honest place to do that.

## The pillars

These four are the spine of the ecosystem — each one a domain bet, all bare-metal:

### HELIOS — *AI × energy*
24/7 predictive DC-microgrid controller. Rust MPPT loop, CNN-LSTM forecasting, post-quantum trust anchors. *Where the lights actually have to stay on.*

### KHAOS — *AI × neuroscience*
Closed-loop BCI kernel. **Sub-100µs CUDA DSP latency**, compile-time-enforced neuroethics, post-quantum cryptography. *Where milliseconds carry weight for the right reasons.*

### SUBSTRATE — *AI × quantum*
Multi-scale physics & quantum-biology simulation. Hand-written CUDA (sm_120) with an honest **kernel-only roofline (3×→154× vs JAX-CPU)** and tensor-network solvers for cryptochrome, EM fields, and multi-body dynamics.

### Blaze — *the compressor*
Tensor-Train / MPS compression for high-order scientific and quantum-state data. GPU SVD, MPS↔circuit bridge. Cross-cuts the ecosystem; also the χ thermometer in [DRIFT](https://github.com/QuantumDrizzy/DRIFT).

---

## A glimpse of the work

[DRIFT](https://github.com/QuantumDrizzy/DRIFT) reads optimization, self-assembly, self-replication, and neural memory (Hopfield, Nobel Physics 2024) as **ground states of one Ising Hamiltonian** — the unification thesis, made measurable:

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/DRIFT/master/figures/phase7_four_faces.png" alt="DRIFT — four faces, one engine" width="720">
</p>

How far is real hardware from the physical floor? **Six orders of magnitude above the Landauer wall.** That gap is the room left for computronium:

<p align="center">
  <img src="https://raw.githubusercontent.com/QuantumDrizzy/DRIFT/master/figures/phase7_roofline.png" alt="cosmic roofline — real hardware vs. Landauer floor" width="720">
</p>

---

## Other open & active work

- **[DRIFT](https://github.com/QuantumDrizzy/DRIFT)** — A microscope for physical computation. Four faces, one Ising engine; tensor-network χ as the compute-density thermometer. P0–P7 done.
- **[TESSERA](https://github.com/QuantumDrizzy/TESSERA)** — Neural-guided real quantum annealing via tensor networks (MPS/TEBD); a GNN learns the schedule on a local GPU.
- **BLACKWALL** — Honest precision-spectrum GEMM roofline on Blackwell (sm_120): **FP32 → FP4 measured, FP4 at 20× FP32 via cuBLASLt**, anchored to the computed peak.
- **EIGEN** — Quantum-inspired threat modeling via transverse-field Ising models and a pure-Rust Lanczos solver.
- **KINECT-NIR** — Real-time IR object detection & tracking. CUDA CA-CFAR kernel + TensorRT INT8 + Kalman filtering.

Several larger systems are in private development and can be discussed in conversation.

---

## Stack

**Systems** — Rust · C · C++ · CUDA (sm_120 Blackwell) · CUDA-Q · Assembly
**Quantum** — Cirq · tensor networks (TT / MPS / TEBD) · QUBO / Ising · Lanczos / Krylov
**AI / ML** — Python · PyTorch · cuBLAS · cuBLASLt · TensorRT · Flash Attention
**HPC / Infra** — SLURM · NCCL · Arch Linux · bare-metal
**Sovereignty** — Post-quantum primitives · compile-time safety · auditable code

---

*Bare-metal · local-first · honest benchmarks · no cloud by default.*
