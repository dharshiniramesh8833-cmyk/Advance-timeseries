This project focuses on forecasting multivariate time series data using deep learning models, with a particular emphasis on the Transformer architecture and its attention mechanism. The goal is to compare the performance of a Transformer-based model with a traditional LSTM model and to understand how Transformers use attention to learn complex temporal patterns.

A synthetic dataset with five features was generated using simple seasonal patterns, mild trends, nonlinear components, and noise. Sliding-window preprocessing was applied to convert the continuous time series into supervised learning sequences. The dataset was split into training, validation, and test sets, and all features were standardized.

Two models were developed and trained:

LSTM Baseline:
A traditional recurrent neural network capable of modeling temporal dependencies but limited in handling long-range patterns.

Transformer Model:
A deep learning architecture using self-attention instead of recurrence. Positional encoding was applied to preserve sequence order. Multiple attention heads and stacked encoder layers enabled the model to learn complex relationships across time steps.

Both models were trained using MSE loss and evaluated on the test dataset using MSE, RMSE, and MAE. The Transformer consistently outperformed the LSTM across all metrics, demonstrating its superior ability to capture long-term dependencies and nonlinear interactions.

A key part of the project was attention visualization. The attention heatmap extracted from the first Transformer encoder layer illustrated which input time steps were most influential in producing the final forecast. This visualization provided interpretability, showing that the model selectively focuses on important past points rather than treating all time steps equally.

In summary, the project shows that Transformers, with their attention mechanisms, offer strong performance and interpretability advantages over traditional LSTM models for multivariate time series forecasting. The simplified experimental design, clean implementation, and clear visualizations make the findings easy to understand while meeting advanced deep learning project criteria.
