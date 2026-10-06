<p align="center">
  <img src="assets/cinema_mycelium.gif" width="820">
</p>

### · [LYTH](https://github.com/QuantumDrizzy/LYTH) — *a kernel that cannot say what it costs does not compile*

A memory-first kernel language for bare-metal HPC and quantum. Movement is declared; arithmetic is
subordinate to it. The intensity written in the source is checked against the one the compiler derives
from the body, and a mismatch does not compile. The accounting is then checked against the silicon,
not against itself: **28.41 B measured by `ncu` against 29.00 counted, 0.98×**.

One `.lyth` file becomes PTX for any NVIDIA GPU from Turing to Blackwell (accepted by `ptxas` on
sm_75 → sm_120, run on sm_120), and the same kernel arrives as a **Rust** module, a **C/C++** header
and a **Python** module, each with its cost contract embedded. Against hand-written CUDA: 17 % more
instructions, the same time.

Quantum circuits are LYTH kernels too: a state vector updated in place, gates fused into one pass over
memory. **A 340-gate circuit drops from 130.31 ms to 38.53 ms (3.38×) with every bit unchanged**, and
circuits agree with Qiskit to ≤ 6.6e-8. Two pre-registered predictions failed, and they stay on the
record.

Open source, MIT OR Apache-2.0. Measure your own GPU, call it from your own code, and send what breaks.
