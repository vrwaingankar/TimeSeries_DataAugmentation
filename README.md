# TimeSeries_DataAugmentation
Exploring Time Series Augmentations Using TSGM Library
1. Time Series Augmentations:
- Time series augmentations are often overlooked in domains outside of computer vision pipelines.
- In this tutorial, we explore time series augmentations using the TSGM library.
- The goal is to produce additional samples that can improve downstream tasks.
- Gaussian noise augmentation adds random noise to time series, making models more robust.
- Shuffling features are useful for multivariate time series with invariant feature permutations.
- Slice and shuffle augmentation cuts and shuffles time series segments.
- Magnitude warping changes the magnitude of each sample in a time series.
- Window warping speeds up or slows down selected windows in time series data.
- DTWBA is an augmentation method based on Dynamic Time Warping.
- Augmentations with generative ML models can generate synthetic time series samples.

2. Gaussian Noise Augmentation:
- Gaussian noise is added to time series to increase robustness and performance.
- The noise parameters can be customized based on the dataset and downstream problem.

3. Shuffle Features:
- Feature shuffling is suitable for multivariate time series with invariant feature permutations.
- It can be used to augment data where features represent independent measurements from sensors.

4. Slice and Shuffle:
- Slice and shuffle augmentation cuts time series into segments and shuffles them.
- This augmentation is useful for time series with invariance over time, such as wearable device data.

5. Magnitude Warping:
- Magnitude warping changes the magnitude of each sample in a time series dataset.
- The magnitude scaling can be beneficial for various applications.

6. Window Warping:
- Window warping speeds up or slows down selected windows in time series data.
- This augmentation can be used to model equipment that changes the speed of change over time.

7. Dynamic Time Warping Barycentric Average (DTWBA):
- DTWBA is an augmentation method based on Dynamic Time Warping (DTW).
- It syncs time series and computes the average of all the computed paths.

8. Augmentation with Generative ML Models:
- Generative ML models can be trained to generate synthetic time series samples.
- Methods like VAEs, GANs, and Gaussian processes are available in the TSGM library.

9. Analyzing Problem Invariances:
- A crucial step in problem analysis is determining if the problem is invariant to random noise and feature shuffling.
- This ensures that the selected methods will improve downstream performance.

Implementing a hybrid model that combines a GAN and VAE (Variational Autoencoder) is a more advanced task. In such a hybrid model, the VAE can help generate more structured and meaningful data, while the GAN can improve the diversity and sharpness of the generated samples.
