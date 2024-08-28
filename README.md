# IEEE Signal Processing Cup 2024 - Team Wavemasters

## 🚀 Project Overview

This project tackles the challenging task of **text-independent far-field speaker recognition** under noise and reverberation conditions, specifically for mobile robots. Our goal is to develop a robust speaker recognition system using advanced signal processing techniques and machine learning algorithms.

## 📝 Project Description

In this project, we focus on creating a system capable of accurately identifying speakers from speech signals captured by mobile robots in challenging acoustic environments. Our approach is composed of the following key components:

- **🎧 Noise Removal and Amplification:**  
  Leveraging **Wavelet Transform** for effective signal denoising.
  
- **📊 Feature Extraction:**  
  Utilizing **Mel-Frequency Cepstral Coefficients (MFCCs)** to extract robust audio features.

- **🛠️ Data Augmentation:**  
  Applying techniques like **Gaussian noise addition, time stretching, pitch scaling,** and **random gain modulation** to expand and diversify the training dataset.

- **🤖 Speaker Recognition:**  
  Implementing the **VGGish pre-trained model** for high-level semantic embedding extraction, tailored for downstream classification tasks.

## 🔍 Methodology

### 1. Wavelet-based Signal Denoising

- **Decomposition:**  
  The audio signal is decomposed into approximation and detail coefficients using Discrete Wavelet Transform (DWT).

- **Thresholding:**  
  Noise is mitigated through soft and hard thresholding techniques applied to the detail coefficients.

- **Reconstruction:**  
  The signal is reconstructed using the modified coefficients, omitting high-frequency details for a cleaner output.

### 2. Feature Extraction

- **Mel-Frequency Cepstral Coefficients (MFCCs):**  
  We extract MFCCs using the `librosa` library, capturing essential characteristics of the audio signals in the frequency domain.

### 3. Data Augmentation

- **Diverse Techniques:**  
  We employ various augmentation techniques such as **Gaussian noise addition, time stretching, pitch scaling,** and **random gain modulation** to generate additional training samples, enhancing the model’s generalization capabilities.

### 4. Model Implementation

- **VGGish Pre-trained Model:**  
  We use VGGish, a model pre-trained on large-scale audio data, to extract **128-dimensional embeddings** from denoised audio signals. These embeddings serve as the input for downstream classification tasks.
