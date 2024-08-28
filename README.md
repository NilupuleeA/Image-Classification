IEEE Signal Processing Cup 2024 - Team Wavemasters
Project Overview
This  contains the code and documentation for our participation in the IEEE Signal Processing Cup 2024. The competition challenges teams to address the problem of text-independent far-field speaker recognition under noise and reverberation conditions for mobile robots. Our team, Wavemasters, approached this challenge by leveraging signal processing techniques and machine learning algorithms to develop a robust speaker recognition system.

Project Description
Our project focuses on developing a robust speaker recognition system capable of accurately identifying speakers from speech signals captured by mobile robots under challenging acoustic environments. The key components of our approach include:

Noise Removal and Amplification: Utilizing Wavelet Transform for signal denoising.
Feature Extraction: Using Mel-Frequency Cepstral Coefficients (MFCCs) for robust feature extraction from audio signals.
Data Augmentation: Applying techniques like Gaussian noise addition, time stretching, pitch scaling, and random gain modulation to enhance the training dataset.
Speaker Recognition: Implementing a VGGish pre-trained model for extracting high-level semantic embeddings for downstream classification tasks.

Methodology
Wavelet-based Signal Denoising:

Decomposition: Signal decomposed into approximation and detail coefficients.
Thresholding: Noise mitigation using soft and hard thresholding techniques.
Reconstruction: Signal reconstructed using modified coefficients, omitting high-frequency details.
Feature Extraction:

Extracting MFCCs using the librosa library to capture essential audio characteristics.
Data Augmentation:

Generating additional audio samples using various augmentation techniques to improve model generalization.
Model Implementation:

Using the VGGish pre-trained model to extract 128-dimensional embeddings from denoised audio signals.
