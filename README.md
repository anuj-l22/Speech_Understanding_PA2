# CSL7770 : Speech Understanding (By Anuj Rajan Lalla [B22AI061])

This repository contains solutions for Speech Understanding tasks across two primary questions.

---

## Q1: Speaker Verification and Speech Enhancement

**Objective:**  
Evaluate a pre-trained speaker verification model on VoxCeleb1 and fine-tune it using VoxCeleb2 with LoRA and ArcFace loss. Performance is compared using metrics such as EER, TAR@1%FAR, and Speaker Identification Accuracy.

**Files:**  
- `B22AI061_PA2_Q1.ipynb` — Jupyter Notebook containing the code for evaluation and fine-tuning.  
- `B22AI061_Speech_PA_Q1.pdf` — Detailed report on the methodology, experimental setup, and results.

**Key Points:**  
- VoxCeleb1 (evaluation) and VoxCeleb2 (fine-tuning) datasets are used.  
- VoxCeleb2 is split into 100 identities for training and 18 for testing.  
- Fine-tuning with LoRA and ArcFace loss improves performance by reducing EER, increasing TAR@1%FAR, and enhancing speaker identification accuracy.  
- Visualizations such as ROC curves and histograms clearly demonstrate the improved discrimination between same- and different-speaker pairs.

---

## Q2: MFCC Feature Extraction and Comparative Analysis of Indian Languages

**Objective:**  
Extract MFCC features from a Kaggle audio dataset of 10 Indian languages, analyze and visualize spectral characteristics, and build a CNN classifier for language identification.

**Files:**  
- `B22AI061_PA2_Q2.ipynb` — Jupyter Notebook covering MFCC extraction, visualization, statistical analysis, and CNN-based classification.  
- `B22AI061_Speech_PA2_Q2.pdf` — Detailed report on the methodology, experimental procedures, and performance evaluation.

**Key Points:**  
- MFCCs are computed for each audio sample and spectrograms are generated for representative languages (e.g., Hindi, Gujarati, Punjabi).  
- Statistical analysis (mean and variance of MFCC coefficients) highlights distinct spectral patterns across the languages.  
- A CNN classifier trained on these features achieves an overall accuracy of approximately 85%, with detailed evaluation through confusion matrices and classification reports.

---

## How to Use

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/YourUsername/YourRepository.git
   cd YourRepository
   ```

2. **Navigate to the Relevant Directory**  
   - For Q1: `cd Q1`  
   - For Q2: `cd Q2`

3. **Install Dependencies**  
   Ensure you have the required Python libraries installed. Refer to the individual README files

4. **Run the Notebooks**  
   Open the respective Jupyter Notebook (e.g., `B22AI061_PA2_Q1.ipynb` or `B22AI061_PA2_Q2.ipynb`) in Jupyter/Colab and follow the in-notebook instructions.

5. **Review the Reports**  
   Detailed reports (`.pdf` files) provide further insights into the experimental setups and results.

---

