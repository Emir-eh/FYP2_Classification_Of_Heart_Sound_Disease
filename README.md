# Classification of Heart Sound Diseases Using Deep Learning

This repository contains the implementation notebooks for my Final Year Project titled **Classification of Heart Sound Auscultation Using Deep Learning for Cardiovascular Disease Detection**.

The project focuses on classifying heart sound recordings using deep learning models. Two types of audio feature representations were used: **MFCC** and **Mel-Spectrogram**. The experiments were conducted using two datasets: the **PASCAL heart sound dataset** and the **Yaseen Khan heart sound dataset**.

## Project Overview

Heart sound auscultation is commonly used to detect possible cardiovascular abnormalities. However, manual interpretation may depend on clinical experience and can be affected by noise or recording quality. Therefore, this project explores the use of deep learning models to automatically classify heart sound recordings into different disease categories.

The main objectives of this project are:

- To extract heart sound features using MFCC and Mel-Spectrogram.
- To train and evaluate several deep learning models for heart sound classification.
- To compare model performance between different datasets, feature types, and model architectures.
- To evaluate the effect of data augmentation on classification performance.

## Datasets Used

### 1. PASCAL Dataset

The PASCAL dataset was used for heart sound classification experiments. The classes include:

- Normal
- Murmur
- Extra Heart Sound
- Extrasystole
- Artifact

### 2. Yaseen Khan Dataset

The Yaseen Khan dataset was also used for classification experiments. The classes include:

- Normal
- Mitral Valve Prolapse (MVP)
- Mitral Stenosis (MS)
- Mitral Regurgitation (MR)
- Aortic Stenosis (AS)

## Feature Extraction Methods

Two feature extraction methods were used in this project:

### MFCC

Mel-Frequency Cepstral Coefficients were used to represent important frequency-based characteristics of heart sound signals.

### Mel-Spectrogram

Mel-Spectrograms were used to represent the time-frequency characteristics of heart sound recordings in image-like format.

## Deep Learning Models

The following deep learning models were implemented and evaluated:

- CNN
- LSTM
- VGG19
- 1D CNN-LSTM
- VGG16-LSTM

Some experiments were conducted using raw data, while others included data augmentation to improve model generalisation and handle class imbalance.

## Repository Structure

```text
Classification_Of_HeartSound_Diseases_Github/
│
├── Models_PASCAL/
│   ├── MFCC_As_Input/
│   └── MelSpectogram_As_Input/
│
├── Models_Yaseen/
│   ├── MFCC_As_Input/
│   └── Mel_Spectogram_As_Input/
│
└── README.md

#Notes

This repository contains the main Jupyter Notebook files used for model training and evaluation. Large files such as datasets, trained model files, audio files, and saved checkpoints are not included in this repository due to file size limitations.

The notebooks are organised based on:

Dataset used
Feature extraction method
Model architecture
Augmented and non-augmented experiments
Tools and Libraries

The project was developed using Python and Jupyter Notebook. The main libraries used include:

TensorFlow / Keras
Librosa
NumPy
Pandas
Matplotlib
Scikit-learn
