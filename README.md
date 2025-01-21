# Deep Neural Model for Detecting Gender Stereotypes in Text

This repository contains the code and resources for the BTP2 project titled **"Deep Neural Model for Detecting Gender Stereotypes in Text"**, conducted under the guidance of **Prof. Jiaul H. Paik** at the **Indian Institute of Technology, Kharagpur**.

---

## Project Overview

The project addresses the challenge of identifying gender stereotypes in text data using **Large Language Models (LLMs)**. The model leverages **QLoRA (Quantized Low-Rank Adaptation)** for fine-tuning, achieving efficient memory usage and competitive accuracy. Our trained model demonstrates a **95.2% classification accuracy**, making strides toward fostering inclusive and unbiased language processing systems.

---

## Key Features

- **Dataset Composition**:
  - IMDb Review Dataset
  - Custom Gender Stereotype Dataset

- **Model Fine-Tuning**:
  - Techniques like QLoRA, LoRA, and Prefix Tuning.
  - Pre-trained on Gemma LLM with fine-tuning to detect stereotypes effectively.

## Results Summary

1. **IMDb Dataset:**
   - **Without fine-tuning:** Initial direct inference on the IMDb dataset yielded an accuracy of approximately 53.78%.
   - **With fine-tuning:** Fine-tuning improved accuracy and precision significantly to **92%** and **91%** respectively.

2. **Custom Gender Stereotype Dataset:**
   - The dataset was split into five parts (df1 to df5) with equal positive and negative labels (stereotypical and non-stereotypical sentences).
   - **Without fine-tuning (direct inference):** Average accuracy of **52.7%** was obtained.
   - **With fine-tuning:** The use of QLoRA achieved an average classification accuracy of **95.2%** and a precision of **92%** for detecting positive stereotypes. This improvement emphasizes the effectiveness of advanced fine-tuning strategies like QLoRA.

3. **Model Configurations and Tuning:**
   - QLoRA was fine-tuned with:
     - Rank = 64 for update matrices.
     - Cosine learning rate scheduler.
   - Retaining punctuation and avoiding stopword removal improved the model's accuracy, as preprocessing techniques like removing stopwords or lowercasing did not yield better results due to the short sentence lengths in the custom dataset.
   - 
## Installation

1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/JaishreeramCoder/Bachelor-Thesis-Project2.git)
