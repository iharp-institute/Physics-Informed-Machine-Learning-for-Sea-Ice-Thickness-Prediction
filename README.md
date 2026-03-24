

** The dataset for this project is publicly available and can be accessed at (https://zenodo.org/records/14752305)**

** The reference for the sea ice model data can be found at https://gmd.copernicus.org/articles/12/3745/2019/ **

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

