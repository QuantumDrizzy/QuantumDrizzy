# Antonio Zambudio

Research Software Engineer focused on high-performance systems.

I design and build performance-critical software in **CUDA**, **Rust** and **C++**, with emphasis on low-latency systems, GPU acceleration and scientific computing.

### Highlights

- **354× wall-clock speedup** on a Lindblad master equation solver using custom CUDA kernels on RTX 5060 Ti (sm_120 Blackwell).
- Built a closed-loop BCI kernel with **<100µs end-to-end latency** at 1000 Hz, including compiler-enforced safety and post-quantum cryptography.
- Designed distributed LLM pretraining infrastructure scaling from single GPU to **multi-node SLURM clusters** (FSDP ZeRO-3, Flash Attention 2, MFU tracking).
- Pure-Rust **Lanczos solver** (Hilbert dim=65,536) for quantum-phase-transition-based threat modeling with native egui dashboard at 60 FPS.

---

### Projects

#### [KHAOS-CORE](https://github.com/QuantumDrizzy/KHAOS)
Closed-loop BCI kernel with CUDA DSP pipeline achieving sub-100µs end-to-end latency at 1000 Hz. Features an electrode-density-invariant 12-qubit quantum representation and three-layer safety enforcement (runtime, compile-time `static_assert`, FPGA hardware watchdog). Includes SHA-256 chained forensic audit ledger and CRYSTALS-Kyber-1024 post-quantum cryptography.
`C++17` `CUDA 12` `CUDA-Q` `Python` `CMake` `OpenSSL`

#### [SUBSTRATE](https://github.com/QuantumDrizzy/SUBSTRATE)
Multi-scale electromagnetic computational framework spanning quantum field theory to geomagnetic civilisational risk. 4 operational modules: Lindblad master equation solver (354× speedup over JAX), radical pair quantum biology, lattice QCD + tensor networks, geomagnetic GNN anomaly detection + RAG pipeline.
`Python` `CUDA (sm_120)` `Rust` `PyTorch nightly cu128` `JAX` `CuPy`

#### [HELIOS-NODE](https://github.com/QuantumDrizzy/HELIOS)
Predictive DC microgrid controller: MPPT P&O loop in Rust (100ms tick), CNN-LSTM irradiance predictor trained on real PVGIS data (8,760h, Murcia), SQLite WAL IPC bridge to Rust controller, real-time egui dashboard. Post-quantum trust anchors (ml-kem, ml-dsa) + SHA-256 chained audit log.
`Rust 1.78` `PyTorch` `SQLite WAL` `egui` `tokio` `ml-kem` `ml-dsa`

#### [SESHAT](https://github.com/QuantumDrizzy/SESHAT)
Quantum-assisted decipherment of Linear A (undeciphered for ~3,700 years) formulated as a QUBO optimisation problem. Simulated Annealing: 100% anchor constraint recovery (51/51). 3-gram Kneser-Ney cross-linguistic LM (Linear B + Luwian + Hurrian): perplexity 8.32. Target sign identified at p=0.79. Paper pending arXiv endorsement.
`Rust` `C++/CUDA` `Python/JAX` `LaTeX`

#### [PROMETHEUS](https://github.com/QuantumDrizzy/PROMETHEUS)
Distributed LLM pretraining framework: PyTorch FSDP ZeRO-3, Flash Attention 2, activation checkpointing (~60% VRAM reduction), sequence packing with zero padding waste, MFU tracking. Scales from single RTX to multi-node SLURM clusters. Configs for Qwen2.5-1.5B (1-4 GPU) and Qwen2.5-7B (4-8 GPU, 24GB VRAM).
`Python` `PyTorch FSDP` `Flash Attention 2` `SLURM` `CUDA`

#### [EIGEN (Q-NAA)](https://github.com/QuantumDrizzy/EIGEN)
Quantum threat landscape analyser modelling 16 national critical infrastructure nodes as a transverse-field Ising Hamiltonian. Threat levels emerge from quantum phase transitions - no rule thresholds. Pure-Rust Lanczos solver (Hilbert dim=65,536, QR+Wilkinson shift). Native egui dashboard at 60 FPS with lock-free watch channel.
`Rust` `Python` `CUDA` `egui/eframe` `tokio` `SQLite` `CuPy`

#### [KINECT-NIR](https://github.com/QuantumDrizzy/KINECT-NIR)
Real-time overhead IR object detection pipeline: CUDA CA-CFAR kernel (9x9, atomicAdd), MobileViT-XT with factorised spatiotemporal attention + BiLSTM, TensorRT INT8 + ONNX (opset 14), Kalman filter (Mahalanobis gating), TLE catalog cross-match via Celestrak/Skyfield. FastAPI + WebSocket dashboard at 30Hz. Arduino Mega hardware bridge for servo slew-to-cue.
`C++17` `CUDA` `PyTorch` `TensorRT INT8` `ONNX` `FastAPI` `Arduino`

---

**Stack:** CUDA · C++17 · Rust · Python · PyTorch · JAX · TensorRT · SLURM · CUDA-Q
