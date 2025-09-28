# TimeGAN–VAE Hybrid Framework for Synthetic Time Series

This repository contains code and experiments for a **TimeGAN–VAE hybrid model** to generate
synthetic supply chain stress index (SCSI) data under **data scarcity** conditions.  
The project replicates real-world disruptions such as the **COVID-19 pandemic (2020–2021)** and the
**2022 recovery period**, showing that hybrid models outperform standalone GANs or VAEs.

---

## 📂 Repository Structure
- `notebooks/`
  - `TimeGan_VAE_PCA_final.ipynb` – Main experiment notebook
- `datasets/` *(optional, if allowed to share)*
  - Sample input/output data for reproducibility
- `requirements.txt` – Dependencies
- `README.md` – Project description
- `LICENSE` – Open source license (MIT)

---

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

---

📂 Data Availability  
The synthetic datasets generated in this project are hosted on a **private Kaggle repository**.  
Access can be provided upon request. Please contact:  

✉️ Jessie jess.tstudent@gmail.com  

The datasets will be released publicly upon acceptance of the IEEE CAI 2026 submission.


## 🔧 Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/YOUR_USERNAME/timegan-vae-synthetic-stress.git
cd timegan-vae-synthetic-stress
pip install -r requirements.txt
