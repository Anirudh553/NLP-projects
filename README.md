# Emotion Classification using BERT (PyTorch)

##  Project Overview
This project performs **multi-class emotion classification** on text using a **fine-tuned BERT model** implemented in **pure PyTorch**.

The notebook demonstrates the complete NLP workflow:
- Exploratory Data Analysis (EDA)
- Manual fine-tuning of a pretrained transformer
- Evaluation using standard classification metrics
- Inference on custom text examples

---

##  Dataset
- **Source:** Hugging Face  
- **Dataset:** emotion-dataset-20-emotions  
- **Classes:** 20 emotion categories  
- **Size:** ~80k sentences  

---

##  Model Details
- **Base model:** `bert-base-uncased`
- **Framework:** PyTorch (no HuggingFace Trainer used)
- **Task:** Multi-class text classification
- **Training:** Fine-tuned on emotion dataset

---

##  Evaluation Metrics
The model is evaluated on a held-out test set using:
- Accuracy  
- Precision (weighted)  
- Recall (weighted)  
- F1-score (weighted)  
- Confusion Matrix visualization  

---

##  Inference
A function `predict_text(text: str)` is implemented to:
- Predict the emotion label
- Return confidence score
- Test on custom user-provided sentences

---

## 🚀 How to Run
1. Open the notebook:
2. Run all cells in **Google Colab** (GPU recommended).
3. View:
- Training logs  
- Evaluation metrics  
- Confusion matrix  
- Sample predictions  

---

## 📎 Repository Contents
- `nlp_banana_1.ipynb` → Complete implementation notebook  
- `README.md` → Project documentation  

---

## 👨‍💻 Author
**Anirudh**

---

## 📚 References
- Hugging Face Transformers  
- BERT: Bidirectional Encoder Representations from Transformers  

