# Speaker Identification Using MFCC
Implemented a Speaker Identification system using Mel Frequency Cepstral Coefficients (MFCCs) as features, and applied a machine learning approach to identify speakers based on these features.

A project, in partial fullfilment of Speech and Image Analysis (SIA) Course, Spring 2024 at Sai University. 

## Project Overview
This project focuses on **Speaker Identification** using **Mel-Frequency Cepstral Coefficients (MFCCs)**. The implementation is based on the methodology outlined in the MathWorks reference: [Speaker Identification using Pitch and MFCC](https://www.mathworks.com/help/audio/ug/speaker-identification-using-pitch-and-mfcc.html).

## Table of Contents
- [Problem Statement](#problem-statement)
- [Implementation](#implementation)
- [Results](#results)
- [References](#references)

## Problem Statement
The goal of this project is to implement a **Speaker Identification system** using **MFCCs** as features and apply a **machine learning** approach to classify speakers. The model aims to match an unknown speaker's voice to a set of known speakers based on recorded speech samples.

### Steps to Follow:
1. **Extract Features:**
   - Compute MFCCs from speech recordings.
2. **Train a Classifier:**
   - Use an **SVM (Support Vector Machine) classifier** with **Radial Basis Function (RBF) kernel**.
3. **Evaluate Performance:**
   - Assess model accuracy using metrics like precision, recall, and F1-score.

## Implementation
### Dataset Used
- **Free Spoken Digit Dataset (FSDD)**
- Contains **3000** audio recordings of spoken digits **(0–9)** by **6 speakers**.
- Each speaker recorded **50 samples** per digit.

### Methodology
1. **Feature Extraction:**
   - Extract **13 MFCC coefficients** per audio sample.
2. **Data Preprocessing:**
   - Normalize features, label encode speakers, and split data (80% train, 20% test).
3. **Model Training:**
   - Use **SVM with RBF kernel** and **Grid Search** for hyperparameter tuning.
   - Achieved **98.17% accuracy** before tuning.
   - **Fine-tuning improved accuracy to 99.17%**.
4. **Evaluation Metrics:**
   - **Confusion Matrix**, **Accuracy**, **Precision**, **Recall**, **F1-Score**.

### Code Implementation
- The full implementation is available on **Google Colab**:  
  [Google Colab Notebook](https://colab.research.google.com/drive/1X_K-pOAXmEm1rt0zhIb3lk3eQ2t68a8a?usp=sharing)

## Results
- **Final Model Accuracy: 99.17%**
- **Confusion Matrix Analysis:**
  - Most speakers were classified correctly.
  - Minor misclassifications observed due to vocal similarities.
- **Key Takeaways:**
  - **Hyperparameter tuning significantly improved accuracy**.
  - **MFCC features are highly effective for speaker recognition tasks**.

## References
1. Free Spoken Digit Dataset: [GitHub Repository](https://github.com/Jakobovski/free-spoken-digit-dataset)
2. IEEE Citation Guidelines:  
   [IEEE Citation Guide](https://ieee-dataport.org/sites/default/files/analysis/27/IEEE%20Citation%20Guidelines.pdf)

## Contributor
- **Priyanka A**  
 

