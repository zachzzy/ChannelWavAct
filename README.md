# Supplementary Material for Rebuttal

### Table 1: Ablation Study on Selective Regularization

| Regularization Strategy | Last Acc (%) | Avg Acc (%) | Forgetting (%) | Time (s) |
| :--- | :---: | :---: | :---: | :---: |
| Magnitude-only (Ours) | 30.2 ± 0.5 | 43.6 ± 0.9 | 16.7 ± 0.5 | 1322.1 |
| Magnitude + Geometry | 30.2 ± 0.6 | 43.7 ± 1.0 | 16.8 ± 0.6 | 1331.5 |
| Geometry-only | 29.6 ± 0.3 | 43.3 ± 1.0 | 17.7 ± 0.4 | 1349.2 |


### Table 2: Ablation Study on Injection Mechanism

| Injection Strategy | Learning Rate Setting | Avg Acc (%) | Forgetting (%) |
| :--- | :--- | :---: | :---: |
| Loss-based Trigger (Ours) | Decoupled (lr * 5) | 41.2 | 45.3 |
| Task-start Injection | Decoupled (lr * 5) | 40.7 | 45.1 |
| Static Allocation (Fixed 10 wavelets) | Decoupled (lr * 5) | 40.0 | 46.3 |
| Loss-based Trigger (Ours) | Standard (lr) | 36.5 | 52.3 |
| Task-start Injection | Standard (lr) | 35.1 | 58.8 |
| Static Allocation (Fixed 10 wavelets) | Standard (lr) | 34.9 | 55.7 |


### Table 3: Ablation Study on Wavelet Selection

| Wavelet Function | Learning Rate Setting | Avg Acc (%) | Forgetting (%) |
| :--- | :--- | :---: | :---: |
| Mexican Hat (Ours) | Standard (lr) | 36.5 | 52.3 |
| DOG | Standard (lr) | 34.9 | 56.1 |
| Mexican Hat (Ours) | Decoupled (lr * 5) | 41.2 | 45.3 |
| DOG | Decoupled (lr * 5) | 41.3 | 48.6 |

### Table 4: Ablation Study on Initialization of New Wavelet

| Initialization | Last Acc (%) | Avg Acc (%) | Forgetting (%) |
| :--- | :--- | :---: | :---: |
| Zero-Init (Ours) | 30.2 ± 0.4 | 43.5 ± 0.9 | 16.4 ± 0.4 |
| Random-Init | 8.7 ± 5.9 | 32.5 ± 5.9 | 21.9 ± 3.6 |

### Table 5: Fair Comparison under Strict Parameter Budget

| Method | Parameters | Last Acc (%) | Avg Acc (%) | Forgetting (%) |
| :--- | :---: | :---: | :---: | :---: |
| ChannelWavAct (Ours) | 1,122,500 | 30.2 ± 0.4 | 43.5 ± 0.9 | 16.4 ± 0.4 |
| Expanded Baseline (Layer3 & Layer4 channels +1) | 1,125,184 | 28.2 ± 0.3 | 40.5 ± 1.0 | 18.5 ± 0.5 |
| Expanded Baseline (Layer3 channels +2) | 1,122,008 | 28.0 ± 0.5 | 40.5 ± 0.8 | 19.2 ± 0.5 |

### Table 6: Regularization Method Comparison (Proposed vs. EWC)

| Regularization Method | Learning Rate Setting | Avg Acc (%) | Forgetting (%) |
| :--- | :--- | :---: | :---: |
| Proposed Magnitude Reg (Ours) | Standard (lr) | 36.5 | 52.3 |
| EWC | Standard (lr) | 35.7 | 55.2 |
| Proposed Reg + EWC | Standard (lr) | 35.6 | 51.9 |
| Proposed Magnitude Reg (Ours) | Decoupled (lr * 5) | 41.2 | 45.3 |
| EWC | Decoupled (lr * 5) | 40.8 | 45.2 |
| Proposed Reg + EWC | Decoupled (lr * 5) | 42.1 | 44.0 |

---

### Figure 1: Fourier Amplitude Evolution during Multi-Frequency Regression

<div align="center">
  <img src="spectral_dynamics.png" width="900" alt="Learning Dynamics">
</div>

### Figure 2: Heatmap of Frequency-Domain Learning Dynamics

<div align="center">
  <img src="spectral_heatmap.png" width="900" alt="Spectral Heatmap">
</div>

---

### Figure 3: Hyperparameter Analysis of Regularization Coefficient ($\lambda$)

<div align="center">
  <img src="reg lambda.png" width="900" alt="Sensitivity of Lambda">
</div>

### Figure 4: Hyperparameter Analysis of Patience Threshold ($P$)

<div align="center">
  <img src="patience threshold P.png" width="900" alt="Sensitivity of P">
</div>

### Figure 5: Hyperparameter Analysis of Relative Margin ($\delta$)

<div align="center">
  <img src="relative margin delta.png" width="900" alt="Sensitivity of Delta (margin)">
</div>

### Figure 6: Hyperparameter Analysis of Injection Number ($\Delta$)

<div align="center">
  <img src="inject number Delta.png" width="900" alt="Sensitivity of Injection Number">
</div>
