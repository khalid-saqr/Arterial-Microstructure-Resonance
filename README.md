# A Resonant Coupling Regime in Pulsatile Arterial Flow

This repository contains the source code and data analysis scripts associated with the manuscript:

**"A resonant coupling regime in pulsatile arterial flow induced by blood microstructure relaxation"**

**Author:** Khalid Saqr  
**Affiliation:** Department of Mechanical Engineering, College of Engineering and Technology, Arab Academy for Science, Technology and Maritime Transport, Alexandria, Egypt.  
**ORCID:** 0000-0002-3058-2705
## Abstract
A theoretical framework is developed to investigate nonlinear pulsatile wave propagation in compliant tubes when blood is modeled as a continuum endowed with a dynamically evolving red-blood-cell microstructure tensor. By coupling multi-harmonic Womersley flow with an anisotropic viscous stress and a relaxation-driven microstructure evolution law, the analysis reveals a distinct coupling regime near $De_{A} \approx 1$ and a structural frequency bottleneck at intermediate Womersley numbers ($\alpha \approx 5-10$). In this regime, microstructural relaxation synchronizes with pulsatile forcing, leading to maximized energy dissipation and pronounced waveform distortion phenomena that are structurally absent in Newtonian descriptions. Regime maps derived from reduced solution-state and phase-state formulations identify three fundamental limits: an isotropic Newtonian regime, a quasi-steady frozen-microstructure regime, and an intermediate resonant coupling zone governed by the parameter set $(\alpha, De_{A}, \chi)$. To place these theoretical diagnostics in physiological context, open-access in vivo arterial pressure measurements are analyzed.

## Repository Contents

### 1. Theoretical Framework
* **File:** `notebooks/PulsatileWavePropagation.ipynb`
* **Description:** Implements the core mathematical model of the study. It solves the governing equations for the microstructure-aware fluid model, generates regime maps, and analyzes waveform distortion phenomena.
* **Key Physics:** Covers the coupling of Womersley flow with relaxation-driven microstructure evolution.

### 2. Physiological Validation
* **File:** `notebooks/ConsistencyWithMIMIC-III.ipynb`
* **Description:** Provides physiological context using open-access data from the MIMIC-III Waveform Database. It processes arterial blood pressure (ABP) measurements to validate theoretical diagnostics.
* **Outputs:** Spectral analysis of in vivo waveforms demonstrating low-order spectral dominance and harmonic content.

## Installation & Requirements

To run these notebooks locally, you will need Python 3 and the following dependencies:

```bash
pip install numpy scipy matplotlib pandas wfdb jupyterlab
```

* **`wfdb`**: Required for accessing and processing physiological signals from PhysioNet (MIMIC-III).
* **`numpy` & `scipy`**: For numerical solvers and FFT operations.
* **`matplotlib`**: For generating the manuscript figures.

## Usage

1.  Clone this repository:
    ```bash
    git clone [https://github.com/your-username/Arterial-Microstructure-Resonance.git](https://github.com/your-username/Arterial-Microstructure-Resonance.git)
    ```
2.  Navigate to the directory:
    ```bash
    cd Arterial-Microstructure-Resonance
    ```
3.  Launch Jupyter Lab:
    ```bash
    jupyter lab
    ```

## Citation

If you use this code or the theoretical framework in your research, please cite the accompanying paper:

> Saqr, K. (2026). A resonant coupling regime in pulsatile arterial flow induced by blood microstructure relaxation. *[Journal Name/Preprint]*.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.
