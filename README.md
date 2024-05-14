# Anomaly-detection-for-multivariate-time-series-using-contrastive-generative-adversarial-networks
Reconstruction-based anomaly detection for multivariate time series using contrastive generative adversarial networks

Problem statement
Given a multivariate time series dataset X ∈ R^(N×d), you need to aim to identify anomalous points without utilizing any known ground truth labels. To detect anomalies, reconstruction errors or equivalent methods are calculated using the input data and should be used to improve your anomaly detection models. Your end goal is to achieve an anomaly detection model with a high F1 Score.

Datasets: https://github.com/elisejiuqizhang/TS-AD-Datasets

TASK 1:
Data Analysis: Load the data into a pandas data frame (or equivalent) and perform Exploratory
Data Analysis (EDA) using Matplotlib or Seaborn. Make sure your visualizations are
meaningful and visually allow you to interpret where the existing anomalies lie in the dataset.


TASK 2:
Implement the following pipeline for your anomaly detection model:
• Data Augmentation: Leverage the properties of MTS (Multivariate Timeseries) and
expand the unexplored input space using a novel method called random mask, which follows
a geometric distribution.
• Generator: This module learns the underlying distribution of normal patterns in MTS and
reconstructs it precisely using a Transformer-based autoencoder.
• Discriminator: This module imposes constraints on the reconstructions within the GAN
framework to better capture normal patterns in MTS.
• Contrastive Learning: This module imposes contrastive constraints on representations of
MTS to enhance the generalization capability of the model, and facilitates joint training of the
Discriminator.



TASK 3:
Implement further anomaly detection models based on the following concepts:
- Principal Component Analysis (PCA)
- Graph Deviation Network (GDN)
- Anomaly Transformer
- One-Class SVM
- Isolation Forest
- Local Outlier Factor
- DBSCAN
- Bonus: Dynamic Time Warping (DTW)
- Bonus: Seasonal Hybrid Extreme Studentized Deviate (S-H-ESD):

TASK 4:
Perform Empirical Analysis between all of these methods. Your analysis should include the
following details visually: F1 Score, Time, AUC Score.

Bonus: Showcase the distributions between normal data, abnormal data, reconstructed normal data
and reconstructed abnormal data. Below is an image to help clarify further:
