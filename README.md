# Transformer-Based Multivariate Time Series Forecasting (PyTorch / Baseline Version)

This repository contains the implementation and outputs for a multivariate time series forecasting project using a Transformer-based architecture.  
Due to environment limitations (missing PyTorch GPU libraries), the generated outputs use a deterministic baseline.  
The full Transformer model is provided in the notebook and can be trained on a local machine or cloud GPU environment.

---

## 📘 Project Overview

The goal of this project is to perform **sequence-to-sequence forecasting** on a synthetic multivariate time-series with:

- **6 correlated features**
- **2500 daily timestamps**
- **Forecast horizon: 14 days**
- **Input window: 60 days**

The project includes:

- Dataset generation  
- Preprocessing & scaling  
- Windowing for seq2seq  
- Transformer model definition (encoder–decoder)  
- Training & evaluation logic  
- Baseline forecast generation (fallback when Transformer cannot train)  
- Metrics (RMSE, MAE)  
- Output files for submission  

---

---

## 🧪 Dataset Details

The synthetic dataset includes:

- Weekly seasonality  
- Annual seasonality  
- Feature-to-feature correlations  
- Added promotional spikes  
- Multi-scale noise  
- Feature-specific trends  

Saved as:multivariate_series.csv


---

## 🧠 Model Description

A Transformer encoder–decoder model was implemented with:

- `d_model = 64`  
- `n_heads = 4`  
- `num_layers = 2` (encoder + decoder)  
- Positional encoding  
- Linear projection layers  
- Teacher forcing during training  
- Autoregressive decoding during inference  

The notebook includes:

- Training loop  
- Validation  
- Test evaluation  
- Attention proxy visualization  

---

## ⚠ Environment Note

Training the full Transformer model requires a working PyTorch environment.  
The execution environment used here lacked required GPU libraries (`libnccl.so.2`), so the repository contains:

- A **deterministic baseline forecast**
- A **placeholder model file**  
- All required **evaluation outputs**  

To train the real Transformer model:


---

## 🧠 Model Description

A Transformer encoder–decoder model was implemented with:

- `d_model = 64`  
- `n_heads = 4`  
- `num_layers = 2` (encoder + decoder)  
- Positional encoding  
- Linear projection layers  
- Teacher forcing during training  
- Autoregressive decoding during inference  

The notebook includes:

- Training loop  
- Validation  
- Test evaluation  
- Attention proxy visualization  

---

## ⚠ Environment Note

Training the full Transformer model requires a working PyTorch environment.  
The execution environment used here lacked required GPU libraries (`libnccl.so.2`), so the repository contains:

- A **deterministic baseline forecast**
- A **placeholder model file**  
- All required **evaluation outputs**  

To train the real Transformer model:


---

## 🧠 Model Description

A Transformer encoder–decoder model was implemented with:

- `d_model = 64`  
- `n_heads = 4`  
- `num_layers = 2` (encoder + decoder)  
- Positional encoding  
- Linear projection layers  
- Teacher forcing during training  
- Autoregressive decoding during inference  

The notebook includes:

- Training loop  
- Validation  
- Test evaluation  
- Attention proxy visualization  

---

## ⚠ Environment Note

Training the full Transformer model requires a working PyTorch environment.  
The execution environment used here lacked required GPU libraries (`libnccl.so.2`), so the repository contains:

- A **deterministic baseline forecast**
- A **placeholder model file**  
- All required **evaluation outputs**  

To train the real Transformer model:
pip install torch torchvision


Then run the notebook locally or in Google Colab / Kaggle GPU.









