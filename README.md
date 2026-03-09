# Simulating-the-Universe-using-Diffusion-Models

This project explores the use of machine learning techniques to analyse cosmological simulation data and generate hydrodynamical simulation maps.

The work focuses on two primary tasks:

• Predicting cosmological parameters directly from simulation maps  
• Generating hydrodynamical simulation maps using diffusion models  

The models were trained and evaluated on the **CAMELS cosmological simulation dataset**, consisting of approximately **15,000 simulation maps at 256×256 resolution**.

The full methodology, results, and discussion are documented in the accompanying report.

---

## Key Results

- Convolutional Neural Network (CNN) achieved approximately **4% error for Ωm** and **2% error for σ8** in cosmological parameter prediction.
- Diffusion models (**DDPM / DDIM**) successfully generated hydrodynamical simulation maps conditioned on gravitational N-body simulations.
- Demonstrated the potential for **machine learning methods to accelerate cosmological simulation analysis**.

---

## Methodology Overview

### Dataset Preparation
- Used the **CAMELS cosmological simulation dataset (~15,000 maps)**.
- Applied normalisation and preprocessing to prepare simulation maps for machine learning training.

### Parameter Inference Model
- Implemented a **Convolutional Neural Network (CNN)** in TensorFlow.
- Trained the model to infer cosmological parameters (**Ωm and σ8**) directly from simulation maps.
- Evaluated model performance using fractional prediction error.

### Generative Modelling
- Implemented diffusion-based generative models (**DDPM / DDIM**) using a **U-Net architecture**.
- Generated hydrodynamical simulation maps conditioned on gravitational N-body simulations.

---

## Repository Contents

- `Simulating_the_Universe_Report.pdf` — Full project report including methodology, experiments, and results.

---

## Technologies Used

- Python  
- TensorFlow  
- NumPy / SciPy  
- Machine Learning (CNNs, Diffusion Models)  
