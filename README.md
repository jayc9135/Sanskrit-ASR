# Sanskrit Automatic Speech Recognition (ASR) System

This project implements an Automatic Speech Recognition (ASR) system for the **Sanskrit language**, designed to convert spoken Sanskrit into text with high accuracy. The system is built using deep learning models and advanced speech processing techniques to handle low-resource languages like Sanskrit.

## Table of Contents
- [Objective](#objective)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Challenges](#challenges)
- [Future Work](#future-work)
- [Contributors](#contributors)

## Objective
The goal of this project is to facilitate the transcription of spoken Sanskrit into text, enabling the preservation and promotion of Sanskrit language and culture, while also making it accessible to researchers, educators, and students.

## Features
- Converts spoken Sanskrit into text with high accuracy.
- Supports diverse dialects and accents in the Sanskrit language.
- Feature extraction using **Mel-frequency cepstral coefficients (MFCCs)**.
- End-to-end ASR model using **CNN** and **RNN** with **CTC loss** for speech-to-text conversion.

## Technology Stack
- **Programming Language**: Python
- **Deep Learning Framework**: TensorFlow, Keras
- **Feature Extraction**: MFCCs
- **Model**: Convolutional Neural Network (CNN), Recurrent Neural Network (RNN)
- **Loss Function**: Connectionist Temporal Classification (CTC)
- **Evaluation Metrics**: Word Error Rate (WER)

## Dataset
The model was trained on a dataset consisting of **78 hours** of Sanskrit speech collected from **27 speakers**. The dataset covers a wide range of dialects and accents, making it versatile for various Sanskrit-speaking populations.

- **Speakers**: 20 male and 7 female
- **Native languages of speakers**: Hindi, Tamil, Kannada, Malayalam, etc.
- **Corpus size**: 46,000 sentences

## Model Architecture
1. **Feature Extraction**: MFCC features were extracted from the speech data.
2. **Model**:
   - A **Convolutional Neural Network (CNN)** layer was used for feature extraction.
   - Followed by a **Recurrent Neural Network (RNN)** layer to capture temporal dependencies.
   - The **CTC Loss Function** was used to handle unaligned sequences between the audio input and the corresponding text.

## Results
- **Word Error Rate (WER)**: The ASR system achieved a **0.44 WER** (44%) on the test dataset, indicating moderate accuracy with room for further improvement.
- The best WER achieved was **0.02** using data augmentation techniques.

## Challenges
- **Low-Resource Language**: Sanskrit is a low-resource language, which made it difficult to gather sufficient data for training.
- **Diverse Accents**: Accounting for multiple dialects and accents required careful tuning of the model.

## Future Work
- Implement **language models** to further improve transcription accuracy.
- Apply advanced techniques such as **Speed Perturbation** and **Spec Augmentation** to enhance model robustness.
- Extend the system to support **real-time transcription** for Sanskrit speech.

## Contributors
- **Jayesh Bafana**
- **Bijal Bharadva**
- **Jay Chaudhari**
- **Pranav Dave**
- **Vinit Jha**
- **Jaanvi Nambiar**
