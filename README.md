# Antonio Zambudio

Research Software Engineer focused on high-performance systems.

I design and build performance-critical software in **CUDA**, **Rust** and **C++**, with emphasis on low-latency systems, GPU acceleration and scientific computing.

### Highlights

- **354× wall-clock speedup** on a Lindblad master equation solver using custom CUDA kernels and tensor networks.
- Built a closed-loop BCI kernel with **<100µs end-to-end latency** at 1000 Hz, including compiler-enforced safety and post-quantum cryptography.
- Designed and implemented distributed LLM pretraining infrastructure scaling from single GPU to multi-node SLURM clusters.

### Projects

#### KHAOS
Closed-loop BCI kernel with CUDA DSP pipeline achieving sub-100µs latency. Features electrode-density-invariant 12-qubit representation and three-layer safety enforcement (runtime, compile-time and FPGA). Includes SHA-256 forensic audit ledger and post-quantum cryptography.

#### SUBSTRATE
Multi-scale simulation framework spanning quantum field theory, radical pair dynamics and geomagnetic analysis. Achieved 354× speedup over JAX on RTX 5060 Ti using custom CUDA kernels and cuTensorNet.

#### HELIOS
Predictive DC microgrid controller combining real-time Rust systems with CNN-LSTM irradiance forecasting. Includes post-quantum security (ML-KEM + ML-DSA) and hardware-ready deployment paths.

#### SESHAT
Combinatorial optimization framework for undeciphered Linear A script using QUBO formulation and Simulated Annealing. Achieved 100% anchor recovery and reduced cross-linguistic perplexity to 8.32.

#### prometheus
Distributed LLM pretraining framework using PyTorch FSDP ZeRO-3, Flash Attention 2 and sequence packing. Supports multi-node training with activation checkpointing and MFU tracking.

#### EIGEN
Quantum-inspired threat modeling system representing critical infrastructure as a transverse-field Ising Hamiltonian. Features a pure-Rust Lanczos solver and real-time egui visualization.

#### KINECT-NIR
Real-time infrared object detection and tracking pipeline with CUDA CA-CFAR, MobileViT-XT, TensorRT INT8 inference and Kalman filtering with TLE catalog cross-matching.

---

**Stack**: CUDA, C++17, Rust, Python, PyTorch, TensorRT, SLURM
