# Natural Language Processing with Disaster Tweets

## Project Overview
This project focuses on a Natural Language Processing (NLP) task to classify whether a tweet describes a real disaster event.
The task is based on the Kaggle competition “Natural Language Processing with Disaster Tweets”, which is a binary classification problem.
We compare traditional NLP baseline models with Transformer-based models (DistilBERT and RoBERTa), and further analyze how different text cleaning strategies affect model performance.

## Models Used
  •	TF-IDF + Logistic Regression (Baseline)
	•	CountVectorizer + Naive Bayes (Baseline)
	•	DistilBERT (Fine-tuning)
	•	RoBERTa (Original Cleaning)
	•	RoBERTa (Modified / Gentler Cleaning Strategy)

## Evaluation Metric
All experiments use F1-score as the primary evaluation metric, which balances precision and recall and is consistent with Kaggle’s official leaderboard scoring.

## Dataset Download Instructions
This project uses the Kaggle dataset
“Natural Language Processing with Disaster Tweets”.
Please download the dataset from:
https://www.kaggle.com/competitions/nlp-getting-started
After downloading, place the files in the project root directory:
project_root/
├── train.csv
├── test.csv
└── sample_submission.csv
Dataset files are not included in this repository.

## Environment & Requirements
	•	Python 3.9+
	•	Google Colab (T4 GPU recommended)

## How to Run
1. Download the dataset and place CSV files in the project root directory.
2. Open and run `DL_M1462004_project.ipynb` in Google Colab.
3. Follow the notebook cells to train models and generate predictions.

## Main libraries:
	•	pandas, numpy, scikit-learn
	•	torch
	•	transformers, datasets
	•	gradio (for demo)
  
## Notes 
	•	Dataset files are not uploaded to this repository.
	•	Model weights are not included to keep repository size small.
	•	All experiments were conducted under the same train/validation split (8:2).
