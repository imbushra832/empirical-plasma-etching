Empirical Process Modeling of Reactive-Ion Plasma
Etching Using Neural Networks and Support Vector
Machines

Executive Summary

This project develops and compares three machine learning models — Multilayer Perceptron (MLP), Radial Basis
Function (RBF), and Support Vector Regression (SVR) — to empirically model and optimize ion-assisted plasma
etching processes in semiconductor fabrication. The models predict four critical process outcomes: etch rate, etch
uniformity, oxide selectivity, and photoresist selectivity. Results show that the RBF network achieved the best
overall Mean Squared Error (MSE), while the SVR model performed best for individual targets, particularly etch
rate and selectivities.


1. Introduction
Plasma etching is a crucial step in semiconductor manufacturing. However, first-principles modeling often falls
short due to the complexity of plasma dynamics. This project uses empirical modeling techniques leveraging
machine learning to establish predictive relationships between input process parameters and output process
characteristics.


3. Dataset
The dataset comprises 53 experimental runs, each with six input parameters and four output responses. All
variables were normalized prior to training.


5. Modeling Methodology
Three different models were implemented and tested: - MLP: Multi-layer perceptron network with Adam optimizer
and early stopping. - RBF: Radial basis function network with Gaussian activations and k-means centers. - SVR:
Support vector regression models optimized for each output response.


7. Results and Analysis
RBF achieved the lowest overall MSE, while SVR yielded the best performance on individual responses,
especially etch rate (R² = 0.9111). All models struggled with predicting etch uniformity, indicating unmodeled
nonlinear effects.


9. Optimization and Sensitivity Analysis
Using the RBF model, optimal parameters were determined to maximize etch rate while minimizing uniformity.
Predicted etch rate improved from 4204 Å/min to 5626 Å/min with uniformity dropping from 11.64% to 5.31%.

11. Discussion
MLP showed balanced results but lacked precision on etch rate. RBF offered the best general performance, while
SVR excelled in target-specific predictions. Findings align with prior literature highlighting the suitability of
empirical ML models for plasma process prediction.


13. Conclusions
The study confirms the effectiveness of machine learning for semiconductor plasma process modeling. RBF
networks provide robust generalization, while SVR is best suited for individual target prediction and optimization.

15. Recommendations
• Use RBF for overall process modeling; SVR for target-specific predictions.
• Include additional parameters to improve uniformity prediction.
• Explore ensemble learning or hybrid models.
• Integrate trained models into process control systems for real-time optimization.

17. References
1. Chinnam, Ding, and May (2000)
2. May, G. S., Huang, J., & Spanos, C. J. (1991)
3. Himmel, C. D., & May, G. S. (1993)
4. Box, G. E. P., Hunter, W. G., & Hunter, J. S. (1978)
