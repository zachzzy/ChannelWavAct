# Supplementary Material for Rebuttal

---

### Table 1: Ablation Study on Selective Regularization

| Regularization Strategy | Last Acc (%) | Avg Acc (%) | Forgetting (%) | Time (s) |
| :--- | :---: | :---: | :---: | :---: |
| Magnitude-only (Ours) | 30.2 ± 0.5 | 43.6 ± 0.9 | 16.7 ± 0.5 | 1322.1 |
| Magnitude + Geometry | 30.2 ± 0.6 | 43.7 ± 1.0 | 16.8 ± 0.6 | 1331.5 |
| Geometry-only | 29.6 ± 0.3 | 43.3 ± 1.0 | 17.7 ± 0.4 | 1349.2 |

---

### Table 2: Ablation Study on Injection Mechanism

| Injection Strategy | Learning Rate Setting | Avg Acc (%) | Forgetting (%) |
| :--- | :--- | :---: | :---: |
| **Loss-based Trigger (Ours)** | **Decoupled (lr * 5)** | **41.2** | **45.3** |
| Task-start Injection | Decoupled (lr * 5) | 40.7 | 45.1 |
| **Loss-based Trigger (Ours)** | **Standard (lr)** | **36.5** | **52.3** |
| Task-start Injection | Standard (lr) | 35.1 | 58.8 |

---

### Figure 1: Fourier Amplitude Evolution during Multi-Frequency Regression

<div align="center">
  <img src="spectral_dynamics.png" width="900" alt="Learning Dynamics">
</div>

---

### Figure 2: Heatmap of Frequency-Domain Learning Dynamics

<div align="center">
  <img src="spectral_heatmap.png" width="900" alt="Spectral Heatmap">
</div>
