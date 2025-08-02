# 📰 TruthGuard: AI-Powered Fake News Detection

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://truthguard.streamlit.app)
[![GitHub Repo stars](https://img.shields.io/github/stars/Ibrahim5570/fake-news-detector-with-feedback?style=social)](https://github.com/Ibrahim5570/fake-news-detector-with-feedback)
![TruthGuard Screenshot](screenshot.png)

TruthGuard is an AI-powered tool that helps users verify news headlines and combat misinformation. By leveraging machine learning, it analyzes linguistic patterns to identify potentially fake news with user feedback to continuously improve accuracy.

# ✨ Features

- 🔍 Real-time headline analysis with confidence scoring
- 📊 Visual model performance metrics and insights
- 💬 User feedback system to correct mistakes
- 🔄 One-click model retraining with new feedback
- 📈 Performance tracking across retraining cycles
- 🌐 Intuitive, user-friendly interface

## 🚀 Try It Live

# COMING SOON!

# 🖥️ Run Locally

## Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/truthguard.git
cd truthguard

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Linux/MacOS
venv\Scripts\activate    # Windows

# Install dependencies
pip install -r requirements.txt

# Download the pre-trained model (or train your own)
# [Add instructions for obtaining model files]
```

# Running the Application
```bash
  streamlit run app.py
  The app will automatically open in your default web browser at http://localhost:8501.
```

# 🤝 How to Contribute

## **We welcome contributions! Here's how you can help:**

* Report issues: Found a bug? Please open an issue with details.
* Suggest features: Have an idea to improve TruthGuard? Create a feature request .
* Contribute code:
* Fork the repository
* Create your feature branch (git checkout -b feature/AmazingFeature)
* Commit your changes (git commit -m 'Add some AmazingFeature')
* Push to the branch (git push origin feature/AmazingFeature)
* Open a Pull Request

# 📦 Project Structure

web-app/

├── app.py                # Main Streamlit application

├── train.py              # Model training script

├── requirements.txt      # Python dependencies

├── models/               # Trained model files

│   ├── fake_news_model.pth

│   └── tfidf_vectorizer.pkl

├── data/                 # Feedback and metrics storage

│   ├── feedback.jsonl

│   └── correct_predictions.jsonl

└── README.md             # This file

# 📜 License

## This project is licensed under the MIT License - see the LICENSE file for details.

# 🙏 Acknowledgments

* Built with Streamlit
* Uses PyTorch for deep learning
* Dataset sourced from Kaggle

# Author

## Ibrahim Abdullah

# Connect with me
---
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ibrahim5570)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ibrahim-abdullah-220917319)


