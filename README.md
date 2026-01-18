Multimodal Personality Prediction for Better Recruitment Decision 🚀

📌 Project Overview
Traditional recruitment often relies heavily on resumes, missing the "human" side of a candidate, or relies on subjective interviews that can be biased.

This project is a Multimodal AI System designed to assist recruiters in hiring Data Scientists. It combines Natural Language Processing (NLP) to analyze resumes and Computer Vision (CV) to analyze behavioral cues from video interviews.The goal is to predict candidate suitability based on both technical skills and personality traits.

🧠 How It Works
The system processes two types of inputs to generate a final "Suitability Score":

1. Resume Analysis (NLP Module) - 60% Weight
   Technique: Uses a hybrid approach of keyword matching and BERT (Bidirectional Encoder Representations from Transformers) embeddings to understand context.
   What it looks for: Analyzes specific sections including Work Experience, Technical Skills (e.g., Python, SQL), Projects, and Education.
   Goal: Assesses the "Technical Fit" of the candidate.

2. Personality Prediction (Computer Vision Module) - 40% Weight
   Technique: Uses Convolutional Neural Networks (CNNs) for Facial Emotion Recognition (FER) on video frames.
   Trait Mapping: Maps micro-expressions and emotion profiles to three key Big Five Personality Traits relevant to data science:
    Conscientiousness: (Focus and discipline).
    Openness: (Curiosity and communication style).
    Emotional Stability: (Calmness under pressure).

3. The Final Decision
   The system fuses the scores ($0.6 \times \text{Resume} + 0.4 \times \text{Personality}$) to classify candidates into categories: Strong Recommend, Recommend , Moderate, or Not Recommend.

📊 Key Results & Performance
This model was tested on a dataset of 80 candidates and outperformed traditional single-method approaches:

| Model Type | Accuracy | Precision | F1-Score |

| Resume Only (NLP) | 70.1% | 0.69 | 0.68 |
| Video Only (CV) | 67.8% | 0.65 | 0.64 |
| Hybrid Model (This Project) | 74.3% | 0.73 | 0.72 |

🛠️ Tech Stack
Language: Python
NLP: Hugging Face Transformers (BERT), NLTK, Pandas
Computer Vision: OpenCV, PyTorch, FER (Facial Emotion Recognition)
Web Interface: Flask (for the demo application)
Visualization: Matplotlib, Seaborn

---
Created by: M.A Ishan Subhashana.
University: General Sir John Kotelawala Defence University (KDU)
