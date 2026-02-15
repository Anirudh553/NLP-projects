# Emotion Classification using BERT (PyTorch)

## 1. Approach
This project performs **multi-class emotion classification** on text using a **fine-tuned BERT model** implemented in **pure PyTorch** (without HuggingFace Trainer).

Workflow followed:
- Loaded the emotion dataset from Hugging Face.
- Performed **Exploratory Data Analysis (EDA)** to inspect class distribution and imbalance.
- Tokenized text using **BERT tokenizer**.
- Manually fine-tuned **bert-base-uncased** using a **custom PyTorch training loop**.
- Evaluated the model on a held-out test set.
- Built an **inference function** to predict emotions for new text.

---

## 2. Assumptions
- The dataset labels correctly represent the underlying emotions.
- A **train–test split of 90:10** is sufficient for evaluation.
- Fine-tuning for **1–2 epochs** is adequate for demonstrating learning in an academic setting.
- Weighted evaluation metrics are appropriate due to slight class imbalance.

---

## 3. Observations
- Training loss **decreased over epochs**, confirming successful fine-tuning.
- The model achieved **reasonable accuracy and F1-score** for a multi-class emotion task.
- Confusion matrix shows that **semantically similar emotions** are occasionally misclassified.
- Using **GPU significantly reduces training time** compared to CPU.

---

## Dataset
- Source: Hugging Face  
- Name: emotion-dataset-20-emotions  
- Size: ~80k text samples  
- Classes: 20 emotion categories  

---

## Model Details
- Base model: `bert-base-uncased`
- Framework: **PyTorch only**
- Task: Multi-class text classification
- Training: Manual fine-tuning loop

---

## Evaluation Metrics
- Accuracy  
- Precision (weighted)  
- Recall (weighted)  
- F1-score (weighted)  
- Confusion Matrix visualization  

---

## Inference
Function implemented:

