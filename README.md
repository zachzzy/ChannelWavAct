# Supplementary Material for Rebuttal

This anonymous repository contains the supplementary high-resolution figures referenced in our rebuttal, specifically addressing the empirical validation of spectral bias and learning dynamics.

---

### Figure 1: Fourier Amplitude Evolution during Multi-Frequency Regression
**Description:** We replicated "Experiment 1" from Rahaman et al. (2019) to track the discrete Fourier amplitude of the network's prediction at specific frequencies (5Hz to 30Hz) over 10,000 iterations.

<div align="center">
  <img src="spectral_dynamics.png" width="900" alt="Learning Dynamics">
</div>

* **Left (Standard ReLU):** Exhibits severe spectral learning bias. High frequencies (25Hz, 30Hz) fail to converge.
* **Right (ChannelWavAct):** Breaks the convergence bottleneck, learning high and low frequencies almost simultaneously.

---

### Figure 2: Heatmap of Frequency-Domain Learning Dynamics
**Description:** A broader frequency-domain analysis (5Hz to 50Hz) over 15,000 training iterations, visualized as a 2D heatmap.

<div align="center">
  <img src="spectral_heatmap.png" width="900" alt="Spectral Heatmap">
</div>

* **Left (Standard ReLU):** The diagonal boundary clearly shows that high-frequency regions (>30Hz) remain poorly fit (dark blue) even after extensive training.
* **Right (ChannelWavAct):** The network uniformly and rapidly illuminates the entire frequency grid in the very early stages of training, explicitly validating the alleviation of spectral bias.
