Natural Language Processing in Cancer: Extracting Diagnostic Insights from Pathology Reports
Project Overview

This project applies Natural Language Processing (NLP) and Transformer-based deep learning techniques to classify cancer pathology reports into multiple cancer types using clinical text data from The Cancer Genome Atlas (TCGA).
The project compares traditional NLP approaches with advanced Transformer models and evaluates their effectiveness in medical text classification.
The system was developed as part of the CSC 590 Master’s Project at California State University, Dominguez Hills.

Objectives

•	Automate cancer type classification from pathology reports
•	Compare traditional NLP models with Transformer-based architectures
•	Evaluate performance using multiple classification metrics
•	Analyze differences between BERT-based models and ChatGPT
•	Improve diagnostic insight extraction from unstructured clinical text

Dataset Information
•	Dataset Source:
-	The Cancer Genome Atlas (TCGA)
•	Dataset Statistics:
•	Description Value
•	Total Reports =   9,523
•	Cancer Types = 32
•	Training Samples = 7618
•	Testing Samples = 1,905
The dataset contains real-world pathology reports with complex clinical terminology and unstructured medical text.

Technologies Used
Programming Language
•	Python

Libraries and Frameworks
•	PyTorch
•	Hugging Face Transformers
•	Scikit-learn
•	Pandas
•	NumPy
•	NLTK
•	Matplotlib

Development Environment
•	Google Colab
•	Jupyter Notebook
•	Visual Studio Code

NLP and Deep Learning Models

1. Bag of Words + Logistic Regression
Traditional NLP baseline model using CountVectorizer for feature extraction.

2. TF-IDF + Random Forest
Weighted text vectorization combined with ensemble decision trees for classification.
3. SciBERT
Transformer model pretrained on scientific research papers for scientific text understanding.

4. BioBERT
•	Transformer model pretrained on biomedical literature and PubMed articles.

5. Ensemble Model
•	Weighted combination of:
-	TF-IDF
-	SciBERT
-	BioBERT
•	The ensemble model achieved the highest overall accuracy.
6. ChatGPT
•	Prompt-based extraction and summarization of:
-	Cancer type
-	Clinical stage
-	Diagnostic summary
Model Performance:
•	Model Accuracy
•	Bag of Words + Logistic Regression = 96.38%
•	TF-IDF + Random Forest = 94.96%
•	SciBERT = 95.85%
•	BioBERT = 95.17%
•	Ensemble Model = 96.75%

Key Features
•	Multi-class cancer classification
•	Medical text preprocessing
•	Transformer-based NLP implementation
•	Ensemble learning
•	Clinical text analysis
•	Classification report generation
•	Confusion matrix visualization
•	ChatGPT-based diagnostic summarization

Project Structure

cancer-pathology-nlp/
│
├── data/
│
├── notebooks/
│   └── NLP_CancerPathology.ipynb
│
├── outputs/
│
├── models/
│
├── screenshots/
│
├── README.md
├── requirements.txt
└── .gitignore

Installation and Setup
Step 1 — Clone Repository

git clone https://github.com/yourusername/cancer-pathology-nlp.git

Step 2 — Open Project Folder
cd cancer-pathology-nlp
Step 3 — Install Required Libraries
pip install -r requirements.txt
Running the Project

Launch Jupyter Notebook
jupyter notebook

Open the notebook:

notebooks/NLP_CancerPathology.ipynb

Run all notebook cells sequentially.


Output and Evaluation

•	The project generates:
-	Cancer type predictions
-	Classification reports
-	Accuracy comparison
-	Confusion matrix visualization
-	Transformer evaluation metrics

BERT vs ChatGPT Analysis

•	This project also compares:
-	Encoder-based Transformer models (SciBERT/BioBERT)
-	Decoder-based generative models (ChatGPT)

•	The analysis highlights architectural and functional differences between:
-	Bidirectional classification models
-	Autoregressive text generation models

Future Work

•	TNM stage prediction
•	Clinical Named Entity Recognition (NER)
- Hyperparameter optimization
- Real-time clinical deployment
- Survival prediction analysis
- Large-scale healthcare integration
