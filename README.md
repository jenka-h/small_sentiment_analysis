# Small Sentiment Analysis -- Growtopia

A deep learning-based sentiment classification project for Growtopia game reviews. This project implements sentiment analysis using multiple training schemes with TensorFlow/Keras, including data collection, preprocessing, model training, and inference capabilities.

## Project Overview

This project performs sentiment classification on Growtopia game reviews using deep learning models. It includes:
- **Web Scraping**: Automated collection of reviews from Google Play Store
- **Data Processing**: Text cleaning and preprocessing with Indonesian language support
- **Model Training**: Multiple training schemes for sentiment classification
- **Inference**: Prediction and sentiment analysis on new reviews

There will be 3 scheme which is:
- Bi-GRU + Embedding
- Bi-LSTM + Embedding
- LinearSVC + TF-IDF

## Project Structure

```
small_sentiment_analysis/
├── pelatihan_model_growtopia.ipynb    # Model training and evaluation notebook
├── scrapping_growtopia.ipynb          # Web scraping notebook for review collection
├── Requirements.txt                   # Project dependencies
├── README.md                          # This file
├── LICENSE                            # MIT License
└── dataset/
    ├── growtopia_dataset_review_raw.csv      # Raw scraped reviews
    ├── growtopia_review_clean.csv            # Cleaned and preprocessed reviews
    └── growtopia_labeled.csv                 # Labeled reviews for training
```

## Dataset

The project uses Growtopia game reviews from Google Play Store with the following files:

| File | Description |
|------|-------------|
| `growtopia_dataset_review_raw.csv` | Raw reviews scraped from Google Play Store |
| `growtopia_review_clean.csv` | Preprocessed and cleaned reviews |
| `growtopia_labeled.csv` | Labeled reviews used for model training |

## Quick Start

### Prerequisites
- Python 3.7+
- pip or conda package manager

### Installation

1. Clone or download the repository
2. Install dependencies:

```bash
pip install -r Requirements.txt
```

### Usage

#### 1. Web Scraping (Collect Reviews)
Open and run `scrapping_growtopia.ipynb` to:
- Scrape reviews from Google Play Store
- Extract review text, ratings, and metadata
- Save raw data to CSV

#### 2. Train Model (Model Training)
Open and run `pelatihan_model_growtopia.ipynb` to:
- Load and preprocess reviews
- Clean and tokenize text
- Train deep learning models with multiple schemes
- Evaluate model performance
- Save trained model for inference

#### 3. Inference (Make Predictions)
Use the trained model to predict sentiment on new reviews

## Dependencies

The project uses the following key libraries:

| Package | Purpose |
|---------|---------|
| **tensorflow** | Deep learning framework for model building and training |
| **scikit-learn** | Machine learning utilities and model evaluation |
| **pandas** | Data manipulation and analysis |
| **numpy** | Numerical computing |
| **nltk** | Natural language processing toolkit |
| **Sastrawi** | Indonesian stemmer for text preprocessing |
| **imbalanced-learn** | Handle imbalanced datasets |
| **google_play_scraper** | Scrape reviews from Google Play Store |
| **matplotlib & seaborn** | Data visualization |

For complete list, see `Requirements.txt`

## Technical Details

### Data Preprocessing
- Text cleaning and normalization
- Indonesian language tokenization using Sastrawi
- Handling imbalanced sentiment classes

### Model Architecture
- Deep learning models built with TensorFlow/Keras
- Multiple training schemes for optimal performance
- Evaluation metrics: accuracy, precision, recall, F1-score

### Workflow
```
Raw Reviews → Data Cleaning → Preprocessing → Model Training → Evaluation → Inference
```

## Author

Jennifer Khang (2026)