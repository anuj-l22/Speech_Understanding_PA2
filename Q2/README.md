# Question 2: MFCC Feature Extraction and Comparative Analysis

This repository contains the code and report for **Question 2** of the PA2. In this task, MFCC features are extracted from an audio dataset of 10 Indian languages, analyzed through visualizations and statistical analysis, and subsequently used for language classification.

## Contents

- **B22AI061_PA2_Q2.ipynb**  
  Jupyter Notebook containing:
  - MFCC extraction from audio samples.
  - Visualization of MFCC spectrograms for representative languages (e.g., Hindi, Gujarati, Punjabi).
  - Statistical analysis of the MFCC features (mean and variance).
  - Implementation and evaluation of a CNN-based language classifier using MFCC features.

- **B22AI061_Speech_PA2_Q2.pdf**  
  The detailed report outlining the methodology, dataset description, MFCC extraction process, visual and statistical analysis, and performance evaluation of the language classifier.

- **README.md**  
  This file, providing an overview of the project, instructions for setup, and usage details.

## Task Description

- **Objective:**  
  Extract and analyze MFCC features from an audio dataset of 10 Indian languages (downloaded from Kaggle).

- **Goals:**
  - Extract MFCCs from each audio sample.
  - Generate and visualize spectrograms for representative samples (e.g., Hindi, Gujarati, Punjabi).
  - Compare MFCC patterns to identify differences and similarities across languages.
  - Compute statistical measures (mean and variance) of the MFCC coefficients.
  - Build and evaluate a Convolutional Neural Network (CNN) classifier to predict the language of an audio sample based on the extracted MFCC features.

## Dataset

- **Source:**  
  Audio dataset with 10 Indian languages from Kaggle.

- **Languages:**  
  Bengali, Gujarati, Hindi, Kannada, Malayalam, Marathi, Punjabi, Tamil, Telugu, and Urdu.

- **Audio Characteristics:**  
  - Each audio sample is approximately 5 seconds long.
  - Original sampling rate is around 44 kHz, which may be resampled during processing.

## Setup and Execution

1. **Clone the Repository**
   ```bash
   git clone https://github.com/anuj-l22/Speech_Understanding_PA2.git
   cd Speech_Understanding_PA2/Q2

2. **Install Dependencies**
   - Ensure you have the necessary Python libraries installed:
     - Librosa, Joblib, Matplotlib, tqdm, NumPy, Scikit-learn, PyTorch, etc.

3. **Prepare the Dataset**
   - Download the audio dataset from Kaggle.
   - Extract and organize the dataset in the expected folder structure as referenced in the notebook.

4. **Run the Notebook**
   - Open the notebook `B22AI061_PA2_Q2.ipynb` in Jupyter or Google Colab.
   - Execute all cells to:
     - Extract MFCC features.
     - Generate and save spectrogram visualizations.
     - Perform statistical analysis on the MFCC coefficients.
     - Train and evaluate the CNN classifier for language classification.

5. **Examine the Results**
   - Check the generated plots and statistical tables within the notebook.
   - Refer to the detailed discussion and conclusions in the report `B22AI061_Speech_PA2_Q2.pdf`.

## Usage

- The notebook guides you through:
  - **MFCC Extraction:** Computing 13 MFCC coefficients (excluding the 0th coefficient) from each audio sample.
  - **Visualization:** Plotting spectrograms for selected samples and generating line/box plots for statistical analysis.
  - **Language Classification:** Preprocessing MFCC features, training a CNN classifier, and evaluating its performance using accuracy, confusion matrix, and classification reports.


