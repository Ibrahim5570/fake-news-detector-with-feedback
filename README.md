# 📰 Fake News Detector

> **A self-learning AI system that detects fake news using machine learning, rule-based logic, and user feedback.**

This project is a **hybrid fake news detection system** built with Python, PyTorch, and TF-IDF. It doesn’t just classify headlines — it **learns from its mistakes and successes**, improving over time through user interaction.

🎯 **No BERT, no GPU required.** Lightweight, explainable, and effective.

---

## 🚀 Live Demo (Coming Soon)
Want to try it without installing?  
👉 [Try the Streamlit Web App](https://your-streamlit-app.huggingface.co) *(Coming soon)*

---

## 🧠 How It Works

This isn’t just a static model — it’s a **self-improving AI system** that combines:

### 1. **Machine Learning (TF-IDF + Neural Network)**
- Uses **TF-IDF vectorization** with 1–3 word n-grams to capture phrases like `"masks cause oxygen loss"`
- A **4-layer neural network** with dropout to prevent overfitting
- Trained on **real data** (`FakeNewsNet.csv`) and **augmented misinformation examples**

### 2. **Rule-Based Filtering**
- Flags **absurd claims** like `"aliens invade Poland"` or `"Queen Elizabeth turns 100"`
- Warns on **sensitive topics** (e.g., health, climate) to encourage fact-checking

### 3. **User Feedback Loop**
- If you disagree with a prediction, you can **correct it**
- If you agree, you **reinforce the model’s confidence**
- All feedback is saved and used in **automatic retraining**

### 4. **Positive Reinforcement**
- The model learns from **both mistakes and correct predictions**
- High-confidence correct predictions are added back as **trusted training data**

### 5. **Auto-Retrain on Exit**
- After every session, the model retrains with new feedback
- Becomes smarter with every use

---

## 🧪 Performance Metrics

After training on **23,208 headlines** (including user feedback), the model achieves:

| Metric | Fake News | Real News |
|-------|----------|----------|
| **Precision** | 0.82 | 0.84 |
| **Recall** | 0.84 | 0.81 |
| **F1-Score** | 0.83 | 0.83 |
| **Accuracy** | 🟢 **83%** (balanced test set) |

✅ Outperforms baseline models and rivals human performance (~60–70%).

---
## 📈 Confusion Matrix and Loss Graph

<img src="visuals\confusion matrix.png"/><br>

<img src="visuals\loss.png"/><br>

---

## 💡 Example Output

```text
📰 Headline: CDC confirms masks cause oxygen loss in children
🔥 Triggered rule: 'masks cause oxygen loss' detected
🎯 Prediction: **Fake News**
📊 Confidence: **95.0%**

📰 Headline: NASA announces new Mars rover launch
⚠️ Warning: This involves a sensitive science topic.
🎯 Prediction: **Real News**
📊 Confidence: **61.2%**

📰 Headline: Aliens invade Poland
🔥 Triggered rule: 'aliens invade' detected
🎯 Prediction: **Fake News**
📊 Confidence: **95.0%**
```

---

# 🛠️ How to Run
## 1. Clone the repo
```bash
  git clone https://github.com/your-username/fake-news-detector.git
  cd fake-news-detector
```

## 2. Install dependencies
```bash
    pip install torch scikit-learn pandas numpy joblib matplotlib seaborn
```
## 3. Run the predictor
```bash
    python predict.py
```
```text
#💡 Type quit, exit, or q to exit and trigger automatic retraining. 
```
---

# Folder Structure
fake-news-detector/

├── FakeNewsNet.csv

├── train.py

├── predict.py

├── models/

│   ├── fake_news_model.pth 

│   └── tfidf_vectorizer.pkl  

├── data/

│   ├── feedback.jsonl

│   └── correct_predictions.jsonl

├── README.md

└── requirements.txt

---
# 🧬 Training Details
* **Model: 4-layer NN: 128 → 64 → 32 → 1, with dropout (0.5)**
* **Loss: Binary Cross-Entropy**
* **Optimizer: Adam (lr=0.001)**
* **Epochs: 2 (to prevent overfitting)**
* **Balanced Data: 50/50 fake vs real (resampled)**
* **Includes: Augmented misinformation, user feedback, and correct predictions**
* **Outputs: Accuracy/loss plots and confusion matrix**

---

# 🚀 Future Roadmap

| **Feature**           | **Status** |
|-----------------------|------------|
| 🖼️ Streamlit Web App | 🔴 Planned |
| 📊 Feedback Dashboard | 🔴 Planned |
|  📱 Mobile App        | 🔴 Planned |

---

# 📈 Why This Matters
## Fake news spreads faster than facts. This project aims to:

* 🔍 Help users think critically about headlines
* 🛠 Build a transparent, explainable AI (no black boxes)
* 🔄 Create a self-learning system that improves with use
* 🎯 Promote media literacy in the age of misinformation
---
# 📄 License
## MIT License

---

# Author 

## Ibrahim Abdullah



# Dataset

### FakeNewsNet.csv (from Kaggle)


# Connect with me

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ibrahim5570)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ibrahim-abdullah-220917319)
