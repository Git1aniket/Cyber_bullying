# Cyber_bullying
cyber bullying tweet project using BERT model 

---

## 🔍 **Project Overview: Cyberbullying Detection using NLP and BERT**

### 📌 **Objective:**

The notebook aims to detect cyberbullying in social media comments using Natural Language Processing (NLP) and fine-tuned BERT (Bidirectional Encoder Representations from Transformers), a powerful transformer-based language model.

---

### 📂 **Dataset:**

* The dataset appears to consist of **text-based social media comments**, each labeled into one of several categories:

  * **Age**
  * **Ethnicity**
  * **Gender**
  * **Religion**
  * **Other Types of Cyberbullying**
  * **Not Cyberbullying**

---

### 🧹 **Data Preprocessing Steps:**

* **Lowercasing**: All text is converted to lowercase.
* **Tokenization & Attention Masks**: The BERT tokenizer is used to convert text into token ids.
* **Truncation & Padding**: Each comment is trimmed or padded to a maximum length for uniformity.
* **Encoding Labels**: Labels are converted into numeric format using one-hot encoding or label encoding.

---

### 🧠 **Model Used:**

* **BERT (Pretrained)**: `bert-base-uncased` from Hugging Face’s Transformers library.
* **Architecture**:

  * Pretrained BERT model
  * Added a classification head (e.g., fully connected layer with softmax)
* **Fine-tuned** on the specific dataset for multi-class classification.

---

### ⚙️ **Training Details:**

* **Loss Function**: CrossEntropyLoss
* **Optimizer**: AdamW
* **Learning Rate Scheduler**: Used for gradual decay of learning rate.
* **Metrics**:

  * Accuracy
  * Precision
  * Recall
  * F1 Score

---

### 📈 **Evaluation:**

* Model is evaluated using a **confusion matrix** and **classification report**.
* Visualization of:

  * Training loss vs. epochs
  * F1 score for each class

---

### ✅ **Strengths:**

* Uses state-of-the-art transformer architecture (BERT)
* Handles multi-class classification effectively
* Covers full pipeline: preprocessing to training and evaluation

---

### 🔚 **Conclusion:**

The notebook successfully implements a transformer-based model for detecting and classifying cyberbullying. The use of BERT ensures contextual understanding of comments, making the model more accurate compared to traditional NLP models.

---

