# 🛡️ Adversarial Attacks and Defenses on Sentiment Analysis (IMDB)

## 📌 Project Overview

This project explores the vulnerability of Natural Language Processing (NLP) models to adversarial attacks and evaluates defense techniques to improve robustness.  
A sentiment analysis classifier is trained on the **IMDB Movie Reviews dataset**, attacked using two different adversarial methods, and strengthened using three defense techniques.

The workflow follows the full adversarial machine learning pipeline:

**Clean Model → Adversarial Attack → Robust Defense**

---

## 📂 Dataset

- **Name:** IMDB Movie Reviews Dataset  
- **Task:** Binary sentiment classification (Positive / Negative)
- **Type:** Text data
- **Samples:** Movie reviews
- **Source:** Standard IMDB sentiment dataset

---

## ⚙️ Project Workflow

1. Dataset loading and preprocessing  
2. Baseline model training and evaluation  
3. Adversarial attack implementation  
4. Defense technique application  
5. Performance comparison and analysis  

---

## 🧠 Model Description

- Supervised machine learning classifier
- Trained on clean IMDB reviews
- Text preprocessing includes:
  - Tokenization
  - Vectorization
  - Train–test split

---

## 📊 Evaluation Metrics

The model is evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

Metrics are reported:
- Before attacks  
- After attacks  
- After defenses  

---

## ⚔️ Adversarial Attacks

Two different adversarial attacks are applied:

### 1️⃣ Synonym Substitution Attack
- Replaces important words with semantic equivalents
- Preserves meaning but changes word surface forms
- Demonstrates semantic-level vulnerability

**Example:**
Original: This movie is amazing
Attacked: This film is astonishing


---

### 2️⃣ Character-Level Noise Attack
- Introduces typos and character substitutions
- Mimics real-world noisy text inputs

**Example:**
Original: The acting was fantastic
Attacked: The act1ng was fantast1c


---

## 🛡️ Defense Techniques

Three defense strategies are implemented:

### 1️⃣ Adversarial Training
- Retraining the model using adversarial examples
- Improves generalization against attacks

### 2️⃣ Regularization
- Reduces overfitting
- Increases model stability

### 3️⃣ Vocabulary Pruning
- Removes rare and noisy tokens
- Enhances robustness to spelling and character noise

---

## 📈 Results Summary

| Model Stage | Performance |
|------------|-------------|
| Before Attack | High accuracy and stability |
| After Attack | Significant performance degradation |
| After Defense | Improved robustness and accuracy recovery |

Defenses successfully mitigate the negative impact of adversarial attacks.

---

## 📁 Repository Structure

├── ULTIMATE_FINAL_Adversarial_IMDB.ipynb
├── Adversarial_IMDB_Report.pdf
├── README.md


---

## 🧪 How to Run

1. Clone the repository:
```bash
git clone https://github.com/hossam-ahmedd/adversarial-imdb.git
```
2.Open the notebook:
```
Adversarial Attacks and Defenses on a Sentiment Analysis Model.ipynb
```
3.Run all cells to reproduce results.

## 📝 Conclusion

**This project demonstrates:**

- How adversarial attacks affect NLP models

- The importance of robustness in real-world systems

- The effectiveness of combining multiple defense techniques

## 📚 References

- IMDB Movie Reviews Dataset

- Adversarial Machine Learning literature

- NLP and Machine Learning resources
