## Question 1: Speech Enhancement

This directory contains code and documentation for **Question 1** of the PA2. The primary objective is to **enhance speech in multi-speaker environments** by focusing on **speaker verification** tasks.

### Contents

- **B22AI061\_PA2\_Q1.ipynb**  
  A Jupyter notebook with the code used for:
  1. Evaluating a pre-trained speaker verification model (\texttt{wavlm-base-plus-sv}) on VoxCeleb1.
  2. Fine-tuning the model using LoRA and ArcFace loss on VoxCeleb2.
  3. Comparing the pre-trained and fine-tuned models with metrics such as EER, TAR@1\%FAR, and Speaker Identification Accuracy.

- **B22AI061\_Speech\_PA\_Q1.pdf**  
  The detailed report describing the methodology, experimental setup, results, and conclusion for Question 1.

- **README.md**  
  The file you are currently reading, which provides an overview of the tasks and how to use the code.

### Task Overview

1. **Dataset Acquisition**  
   - Download VoxCeleb1 (evaluation) and VoxCeleb2 (fine-tuning) from the provided links.
   - VoxCeleb1 is used to evaluate the speaker verification performance, while VoxCeleb2 is used to fine-tune the model.

2. **Speaker Verification**  
   - A pre-trained model (\texttt{wavlm-base-plus-sv}) is evaluated on VoxCeleb1 using:
     - **Equal Error Rate (EER)**
     - **TAR@1\%FAR**
     - **Speaker Identification Accuracy**

3. **Fine-Tuning**  
   - LoRA (Low-Rank Adaptation) and ArcFace loss are used to fine-tune the model on VoxCeleb2.
   - The first 100 speaker identities (sorted in ascending order) are used for training, and the remaining 18 for testing.

4. **Comparison**  
   - The performance of the fine-tuned model is compared with the pre-trained baseline to assess improvements in speaker verification metrics.

### Usage

1. **Clone this Repository**
   ```bash
   git clone https://github.com/anuj-l22/Speech_Understanding_PA2.git
   cd Speech_Understanding_PA2/Q1
   ```

2. **Install Dependencies**
   - Make sure you have the necessary Python libraries installed (e.g., `transformers`, `torch`, `librosa`, `soundfile`, `pydub`, `numpy`, `matplotlib`, `tqdm`, `scikit-learn`, and `peft`).  
  

3. **Prepare the Datasets**
   - Download and extract the VoxCeleb1 and VoxCeleb2 datasets into directories named `vox1` and `vox2`, respectively.
   - Ensure your folder structure matches the paths used in the code (e.g., `vox1/wav`, `vox2/aac`).

4. **Run the Notebook**
   - Open and run **B22AI061\_PA2\_Q1.ipynb** in Jupyter or Google Colab.  
   - Adjust any paths in the notebook to match your local environment.

5. **Examine the Results**
   - The notebook will output metrics (EER, TAR@1\%FAR, Accuracy) and generate ROC curves and histograms showing the distribution of similarity scores for both the pre-trained and fine-tuned models.
   - Refer to **B22AI061\_Speech\_PA\_Q1.pdf** for a complete discussion of the results.
