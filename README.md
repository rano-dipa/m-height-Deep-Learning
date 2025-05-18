# m-height-Deep-Learning
Predicted the m-height h_m(C) of linear codes using deep learning, bypassing costly LP solvers. Trained models on generator matrices and parameters (n, k, m), achieving accurate log-scale predictions with group-specific architectures and transformer variants.

# M-Height Prediction Using Deep Learning

The **m-height problem** in coding theory involves estimating the minimum number of non-zero positions (called **m-height**, denoted \( h_m(C) \)) in the sum of any \( m \) codewords from a linear code \( C \).

Traditionally, this is solved using **linear programming (LP)**, which becomes computationally expensive as code size grows.

In this project, we develop a **deep learning-based solution** that predicts \( h_m(C) \) directly from a linear code's **generator matrix \( G \)** and its parameters \( (n, k, m) \). The models are trained on LP-generated ground truth, allowing **fast and accurate inference** without solving LPs at runtime.

---

## Features

- Predicts **m-height \( h_m(C) \)** from code parameters and generator matrix
- Uses **neural networks**, including:
  - Feedforward Networks
  - Transformer-based Models
  - Set Transformers (permutation-invariant)
-  **Per-group models** trained for each \((n, k, m)\) combination
- **Log-scale loss** for stable and effective training
-  Eliminates need for LP during inference, greatly reducing compute time



