# Abstract
Accurate, non-invasive monitoring of cerebral blood flow is essential for advancing functional neuroimaging and understanding neural dynamics under cognitive stimulus. Traditional imaging methods are limited by cost, invasiveness, and poor temporal resolution, creating a need for more accessible, real-time alternatives.

This project aimed to evaluate whether laser speckle imaging, in combination with machine learning techniques, could classify brain states, relaxing versus visually stimulated, based on hemodynamic fluctuations in the occipital lobe. The study also explored the viability of convolutional neural networks on a small neuroimaging dataset, despite their known data dependency.

Raw LSI data was processed using three signal extraction techniques: Optical Flow, Cross Correlation, and Contrast Correlation. These one-dimensional time series were classified using Support Vector Machine, Random Forest, and Convolutional Neural Network architectures, ResNet-18 and VGG19. Dimensionality reduction via Principal Component Analysis and Relief-F optimised traditional classifiers. Convolutional Neural Networks were trained on image-based inputs from time-series plots and spectrograms.

Contrast Correlation paired with Support Vector Machine under an RBF kernel achieved the highest accuracy at 94.60%, while Random Forest using the same data reached 89.19%. In contrast, Convolutional Neural Networks underperformed (≤65.38%), showing poor generalisation due to dataset size. These findings confirm the discriminative strength of contrast-based temporal features and highlight the limitations of deep learning models on low-volume neuroimaging data.

This study demonstrates that using pre-processed LSI data, lightweight machine learning classifiers can accurately infer cognitive brain states. It lays the foundation for non- invasive, remote neuroimaging systems, with future applications in cognitive monitoring, brain-computer interfaces, and neurodiagnostics.
