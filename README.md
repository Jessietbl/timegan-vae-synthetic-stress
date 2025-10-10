# TimeGAN–VAE Hybrid Framework for Synthetic Time Series

This repository contains code and experiments for a **TimeGAN–VAE hybrid model** to generate
synthetic supply chain stress index (SCSI) data under **data scarcity** conditions.  
The project replicates real-world disruptions such as the **COVID-19 pandemic (2020–2021)** and the
**2022 recovery period**, showing that hybrid models outperform standalone GANs or VAEs.

---

## 📚 Overview

| Component | Description |
|------------|-------------|
| **TimeGAN** | Captures temporal and sequential dependencies for dynamic, volatile variables (e.g., jet fuel price, freight index). |
| **VAE** | Models distributional smoothness and stability for regulated or steady variables (e.g., diesel price, domestic supply). |
| **Hybrid (TimeGAN + VAE + PCA)** | Combines both generative advantages and reduces overfitting, producing a balanced synthetic SCSI for 2019–2024. |

The hybrid approach provides realistic, interpretable, and reproducible synthetic data suitable for supply-chain analytics research.

The hybrid approach provides realistic, interpretable, and reproducible synthetic data suitable for supply-chain analytics research.

## 📂 Repository Structure
- `notebooks/`
  - `TimeGan_VAE_PCA_final.ipynb` – Main experiment notebook
  - `TimeGan_only.ipynb` –  TimeGAN-only experiment
  - `VAE_only.ipynb` – VAE-only experiment
- `datasets/` *(optional, if allowed to share)*
  - Sample input/output data for reproducibility
- `requirements.txt` – Dependencies
- `README.md` – Project description
- `LICENSE` – Open source license (MIT)

---

Each notebook is self-contained:

- TimeGAN-only focuses on sequence realism and temporal learning.
- VAE-only focuses on statistical stability and low-variance reconstruction.
- Hybrid integrates both outputs, applies PCA, and generates the Supply Chain Stress Index (SCSI).
Together, they form a reproducible framework for evaluating generative models under data-scarce Malaysian supply-chain conditions.

## 🚀 Key Features
- **TimeGAN**: Captures temporal patterns in time series.  
- **VAE**: Ensures distributional stability and robustness.  
- **Hybrid TimeGAN–VAE**: Balances both strengths for reliable synthetic data.  
- Application: Supply Chain Stress Index (SCSI) construction under scarce data.  

---

## 📊 Results
- Hybrid TimeGAN–VAE replicates crisis and recovery patterns observed in real data.  
- Outperforms standalone TimeGAN and VAE on:  
  - **Distributional similarity** (Wasserstein distance, KS-test).  
  - **Temporal fidelity** (visual + statistical alignment).  
All experiments are fully reproducible using Google Colab (T4 GPU runtime).

---

📂 Data Availability  
The synthetic datasets generated in this project are hosted on a **private Kaggle repository**.  
Access can be provided upon request. Please contact:  

✉️ Jessie jess.tbl@gmail.com
✉️ Dr Sarah sjsflora@unimas.my

✅ This repository supports open, transparent, and reproducible research in Generative AI for data-scarce environments.

## 🔧 Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/YOUR_USERNAME/timegan-vae-synthetic-stress.git
cd timegan-vae-synthetic-stress
pip install -r requirements.txt
