# Sentiment Analysis of IMDB Movie Reviews

## Overview
This project focuses on sentiment analysis using the IMDB Movie Reviews dataset. We compare traditional machine learning models (Logistic Regression, Naïve Bayes) with deep learning models (RNN, LSTM, GRU) to determine the best approach for classifying reviews as positive or negative.

## Dataset
- **Source:** IMDB dataset from Kaggle
- **Size:** 50,000 reviews (balanced: 25,000 positive, 25,000 negative)
- **Columns:** `review` (text) and `sentiment` (label: positive/negative)
- **Preprocessing:** Tokenization, stopword removal, lemmatization, and feature extraction using TF-IDF and Word2Vec

## Models Implemented
### Traditional ML Models
- **Logistic Regression** (TF-IDF features)
- **Naïve Bayes** (TF-IDF features)

### Deep Learning Models
- **RNN**
- **LSTM**
- **GRU**


## How to Use
### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/sentiment-analysis.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the Colab notebook:
   - Link: [Colab Notebook](https://colab.research.google.com/your-notebook-link)

### Running the Models
- Execute the notebook cells step by step.
- Modify hyperparameters as needed.
- Evaluate results using accuracy, precision, recall, and F1-score.

## Future Improvements
- Fine-tune deep learning models with transformers like BERT.
- Optimize hyperparameters for better performance.
- Expand the dataset with additional review sources.

## Contributors
- **Pierrette Umutoniwase** - Data exploration & preprocessing
- **Aime Magnifique Ndayishimiye** - Traditional ML model implementation
- **Johnson Noe Tuyishime** - Deep learning model implementation

## References
- [AWS Sentiment Analysis](https://aws.amazon.com/what-is/sentiment-analysis/)
- [IMDB Movie Reviews Dataset](https://www.kaggle.com/code/lakshmi25npathi/sentiment-analysis-of-imdb-movie-reviews)

