## Introduction
Accurate prediction of Arctic Sea Ice Thickness (SIT) is a cornerstone of global climate modeling, yet it remains one of the most challenging variables to project. Traditional numerical models are computationally expensive and often struggle with sub-grid scale parameterizations, while 'black-box' deep learning models frequently violate fundamental physical laws, such as energy conservation. My work bridges this gap by developing a Physics-Informed Machine Learning (PIML) framework. 
## Background
# Physics-informed machine learning for sea ice thickness prediction (PhySIT)

### Core Features
* **Proposed hybrid architecture** based on recurrent neural networks (RNNs) for nonlinear spatio-temporal modeling.
* **Integration of Kolmogorov–Arnold Networks (KAN)** to capture complex nonlinear relationships.
* **Framework named PhySIT** (Physics-informed machine learning for sea ice thickness prediction).
* **Use of Layer-Wise Relevance Propagation (LRP)** to improve model interpretability.
* **Enables understanding** of how physics-based features influence predictions.

### Contributions
* **Advancing physics-informed machine learning** specifically within the domain of sea ice modeling.
* **Improving transparency and interpretability** of deep learning models for reliable decision-making.

## ## Dependency
Before running the code, make sure to install the necessary dependencies. **PyTorch** is used for GPU-accelerated tensor operations and neural network functionalities.
## References

[1] A. Sampath, O. Faruque, A. Khan, V. Janeja and J. Wang, "Physics-Informed Machine Learning for Sea Ice Thickness Prediction," 2024 IEEE International Conference on Knowledge Graph (ICKG), Abu Dhabi, United Arab Emirates, 2024, pp. 325-333. doi: [10.1109/ICKG63256.2024.00048](https://doi.org/10.1109/ICKG63256.2024.00048).

# Notes for Replicate this work

### Model Baselines
* **`PGNN_Baseline_Model.ipynb`**: Implementation of the **Physics-Guided Neural Network**. This model integrates physical constraints into the loss function to ensure predictions remain consistent with geophysical laws.
* **`PcudnnLSTM_Baseline_Model.ipynb`**: A high-performance baseline utilizing **cuDNN-optimized LSTM** layers for efficient sequential data processing.
* **`Transformer_Baseline_Model.ipynb`**: A self-attention-based **Transformer** architecture used to capture long-range dependencies in climate variables.

### Ablation Studies
* **`Ablation-KAN-Nophy-LSTM_GRU.ipynb`**: A comparative study of **Kolmogorov-Arnold Networks (KAN)** versus standard **LSTM/GRU** units, specifically removing physics-based constraints to isolate architectural performance.
* **`Ablation-optimizers.ipynb`**: An analysis of how different optimization algorithms impact the convergence and stability of the thickness prediction models.

### Explainability & Interpretability
* **`LRP-GRUU_LSTM.ipynb`**: Employs **Layer-wise Relevance Propagation (LRP)** to visualize and attribute importance to specific input features, "opening the black box" of the GRU and LSTM models.

