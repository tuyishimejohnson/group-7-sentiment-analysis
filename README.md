# Sentiment Analysis of IMDB Movie Reviews

## Overview
This project focuses on sentiment analysis using the IMDB Movie Reviews dataset. We compare traditional machine learning models (Logistic Regression, Naïve Bayes) with deep learning models (RNN, LSTM, GRU) to determine the best approach for classifying reviews as positive or negative.

## Dataset
- **Source:** IMDB dataset from Kaggle
- **Size:** 50,000 reviews (balanced: 25,000 positive, 25,000 negative)
- **Columns:** `review` (text) and `sentiment` (label: positive/negative)

 ## Preprocessing

Text data is rarely "clean" when it comes straight from the source. To prepare it for machine learning and deep learning, we followed these steps:
✔ Removing special characters, HTML tags, and punctuation – to keep only useful words.
✔ Tokenization and padding– breaking down sentences into individual words. This step helps in creating input sequences for the models. A padding sequence function is also used to ensure that all sentences have the same length. In this project, it is crucial for handling variable-length input and enables efficient batch processing.
✔ Stopword Removal – filtering out common words like "the," "is," and "a" that don’t contribute to sentiment.
✔ Lemmatization – reducing words to their root forms (e.g., "running" → "run").
✔ Word Embeddings – converting words into numerical vectors (TF-IDF for ML models, Word2Vec for DL models)

## Models Implemented
### Traditional ML Models

- **Logistic Regression** (TF-IDF features)
- **Naïve Bayes** (TF-IDF features)
- **SVM** (Unfortunately we didn't experiment on it as It was taking too much time to understand and optimize. We plan to try it next time when we have enough time to analyze its performance and fine-tuning it properly.)

### Deep Learning Models
- **RNN**
- **LSTM**
- **GRU**

## Performance 

Logistic Regression was the most effective model for classifying IMDB reviews, achieving the highest accuracy (88.49%), precision (89%), and recall (88%), outperforming deep learning models. Naïve Bayes also performed well with 85.16% accuracy but struggled to capture sentiment nuances due to its assumption of word independence. Among deep learning models, GRU achieved the best performance with 83.5% accuracy and the highest recall (84%), while LSTM and RNN underperformed with recall values of 73% and 74%, respectively. The results suggest that deep learning models, despite their ability to capture sequential data, did not outperform simpler models, likely due to the small dataset size.

## How to Use
### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/tuyishimejohnson/group-7-sentiment-analysis.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the Colab notebook:

### Running the Models
- Execute the notebook cells step by step.
- Modify hyperparameters as needed.
- Evaluate results using accuracy, precision, recall, and F1-score.

## Future Improvements
- Fine-tune deep learning models with transformers like BERT.
- Optimize hyperparameters for better performance.
- Expand the dataset with additional review sources.

## Contributors
- 👩‍💻**Pierrette Umutoniwase** - Data exploration & preprocessing
- 👨‍💻**Aime Magnifique Ndayishimiye** - Traditional ML model implementation
- 👨‍💻**Johnson Noe Tuyishime** - Deep learning model implementation

## References
- [AWS Sentiment Analysis](https://aws.amazon.com/what-is/sentiment-analysis/)
- [IMDB Movie Reviews Dataset](https://www.kaggle.com/code/lakshmi25npathi/sentiment-analysis-of-imdb-movie-reviews)

