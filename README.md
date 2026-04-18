# Hi, I'm Antonio 👋🏻

**Data Scientist · Complex Signals & Applied ML**  
📍 Murcia, Spain · Remote · Open to relocation: Switzerland

---

## About me

Self-taught data scientist with a focus on complex signal analysis and applied ML across scientific domains. Projects span computational neuroscience, geophysics, astronomy, bioinformatics, and quantum ML.

Methodological honesty is a core practice — all results are reported with their limitations and validated without data leakage.

Currently studying Computational Neuroscience (University of Washington) and completing IBM + Google certification stack.

---

## 🛠️ Tech Stack

**Languages**  
Python · SQL · R · Bash · REST APIs

**ML & Signals**  
scikit-learn · PyTorch · MNE · antropy · EEG/LFP pipelines · time-series analysis

**Quantum ML**  
PennyLane · Cirq · VQC · PEPS tensor networks · CUDA-Q

**Gen AI & RAG**  
FAISS · RAG pipelines · ReAct agents · prompt engineering

**Engineering**  
ETL pipelines · SQLite · SQLAlchemy · FastAPI · MLOps · feature stores · Kafka

**Ecosystem**  
Git/GitHub · Jupyter · Google Cloud · IBM Watson · JAX · Plotly · Folium

---

## 📁 Portfolio

### ⚡ Epileptic Seizure Detection — CHB-MIT
Clinical EEG analysis on paediatric focal epilepsy (PhysioNet CHB-MIT, neurologist-annotated).

- Leave-One-Seizure-Out validation: **F1 = 0.945** (interictal vs ictal)
- Preictal prediction: **F1 = 0.883**
- Cross-patient generalisation without retraining: F1 = 0.09–0.41 — each brain has unique seizure signature
- LZC complexity trajectory confirms preictal hypersynchrony · H-H simulation arc: p = 0.0016

`MNE` `scikit-learn` `antropy` `SVM` `Hodgkin-Huxley`

[![Repo](https://img.shields.io/badge/GitHub-eeg--epilepsy-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/eeg-epilepsy)

---

### 🧠 EEG Motor Imagery BCI Pipeline
4-stage pipeline on PhysioNet EEGBCI (64 channels, 160 Hz, 10 subjects).

- CSP + SVM: **99–100%** on 2-class motor imagery
- EEGNet CNN: **62%** on 4-class
- VQC (PennyLane): **45–54%** · Barren plateau documented

`MNE` `EEGNet` `PennyLane` `PyTorch` `CSP`

[![Repo](https://img.shields.io/badge/GitHub-eeg--pipeline-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/eeg-pipeline)

---

### 🔬 Computational Neuroscience — H-H + LZC
Biophysics + information theory applied to neural signals.

- Hodgkin-Huxley model from scratch (4 ODEs, RK45) — action potential, f-I curve, 20-neuron network
- LZC applied to simulation, motor imagery EEG, and epileptic EEG
- Sample Entropy resting vs motor: p = 0.0043 · LZC: p = 0.0412

`scipy` `antropy` `NumPy` `Matplotlib`

[![Repo](https://img.shields.io/badge/GitHub-comp--neuro--projects-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/comp-neuro-projects)

---

### 🌍 Global Seismic Activity — USGS + NOAA
**106,358** real earthquakes (M≥5.0, 1900–2026) cross-referenced with NOAA validated tsunami catalogue.

- Shallow earthquakes generate tsunamis **×14** more frequently than deep (Chi-square p < 0.001)
- Gradient Boosting AUC = **0.725** — pre-event features only, no leakage

`pandas` `folium` `SQLite` `scipy` `Gradient Boosting`

[![Repo](https://img.shields.io/badge/GitHub-seismic--activity--analysis-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/seismic-activity-analysis)

---

### 🪐 Exoplanet Classification — NASA Kepler DR25
9,564 Kepler Objects of Interest — confirmed planets vs false positives using physical observables only.

- koi_score excluded (data leakage) — corrected **AUC = 0.94** (Random Forest)
- 14 confirmed planets in habitable zone

`pandas` `scikit-learn` `scipy` `Random Forest`

[![Repo](https://img.shields.io/badge/GitHub-kepler--exoplanet--analysis-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/kepler-exoplanet-analysis)

---

### ⚛️ ARC-QRL-PEPS Solver — ARC-AGI-3
Quantum Reinforcement Learning agent with PEPS tensor networks for the ARC-AGI-3 Kaggle competition.

- Energy-Based Model with triplet margin loss + MCMC Metropolis-Hastings inference
- 25 environments via official ARC-AGI SDK · JAX/optax training loop
- Proof of concept in active development

`JAX` `PennyLane` `optax` `PEPS` `Metropolis-Hastings`

[![Repo](https://img.shields.io/badge/GitHub-arc--qrl--peps--solver-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/arc-qrl-peps-solver)

---

### 🔭 Quantum Geo-Metrology — IGRF-14
Quantum feature maps applied to IGRF-14 magnetic pole trajectory data (North Pole 2005).

`PennyLane` `Cirq` `NumPy` `scikit-learn`

[![Repo](https://img.shields.io/badge/GitHub-quantum--geo--metrology-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/quantum-geo-metrology)

---

### 🇪🇸 Spain Situation Room — Real-Time Dashboard
Live 3D dashboard: 400+ flights (OpenSky), electricity prices (E·SIOS), weather radar (RainViewer).

`Next.js` `TypeScript` `Deck.GL` `MapLibre` `Kafka`

[![Repo](https://img.shields.io/badge/GitHub-spain--situation--room-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/spain-situation-room)

---

### ✈️ Aviation ETL Pipeline
49 airports · 30 airlines · 1,936 routes · 15,000 flights into SQLite star schema (Kimball modelling).

`pandas` `SQLAlchemy` `SQLite` `ETL`

[![Repo](https://img.shields.io/badge/GitHub-aviation--etl--pipeline-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/aviation-etl-pipeline)

---

### 🌬️ Wind Turbine Predictive Maintenance — MLOps
Full MLOps pipeline: versioned feature store, experiment tracking, model registry, CI/CD design.

`scikit-learn` `MLflow` `TimeSeriesSplit` `Feature Store`

[![Repo](https://img.shields.io/badge/GitHub-wind--turbine--mlops-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/wind-turbine-mlops)

---

### 🤖 Scientific Paper Q&A — RAG Pipeline
30 arXiv papers · FAISS indexing · ReAct agent with tool use · Precision@3 = 0.73

`FAISS` `scikit-learn` `RAG` `ReAct`

[![Repo](https://img.shields.io/badge/GitHub-rag--scientific--papers-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/rag-scientific-papers)

---

### ⚡ IoT Anomaly Detection + FastAPI
50,000 sensor readings · Isolation Forest AUC ~0.85 (honest benchmark on synthetic data) · FastAPI REST service · PSI drift monitoring

`scikit-learn` `FastAPI` `Isolation Forest`

[![Repo](https://img.shields.io/badge/GitHub-iot--anomaly--detection-181717?style=flat&logo=github)](https://github.com/QuantumDrizzy/iot-anomaly-detection)

---

## 📚 Currently

- Computational Neuroscience — University of Washington / Coursera
- IBM Professional Certificates (Data Science · Data Engineering · AI Engineering · ML Engineering · GenAI)
- Google Advanced Data Analytics
- German: active study

---

## 📫 Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/antonio-rodr%C3%ADguez-9bb538220/)
[![Email](https://img.shields.io/badge/ProtonMail-8B89CC?style=flat&logo=protonmail&logoColor=white)](mailto:drizzyrdrgz.exe@protonmail.com)

---

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=QuantumDrizzy&show_icons=true&theme=github_dark&hide_border=true&count_private=true" />
</div>
