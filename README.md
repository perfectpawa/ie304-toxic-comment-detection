# Toxic Comment Detection

This project implements a machine learning model to detect toxic comments in Vietnamese text. The model uses PhoBERT, a pre-trained language model for Vietnamese, to classify comments into different categories of toxicity.

## Project Structure

```
.
├── Dataset.csv              # Main dataset containing comments and labels
├── Abbreviations.csv        # Dictionary of Vietnamese abbreviations
├── vietnamese-stopwords.txt # List of Vietnamese stopwords
├── toxic_comment_detect.ipynb # Main Jupyter notebook with implementation
└── scripts/                 # Additional utility scripts
```

## Features

- Vietnamese text preprocessing using VnCoreNLP
- Abbreviation normalization
- Toxic comment classification using PhoBERT
- Support for multiple toxicity levels (0: Non-toxic, 1: Mildly toxic, 2: Highly toxic)

## Requirements

- Python 3.x
- PyTorch
- Transformers
- VnCoreNLP
- pandas
- numpy
- scikit-learn
- unidecode

## Data Format

The dataset contains the following columns:
- Id: Unique identifier for each comment
- Label: Toxicity level (0, 1, or 2)
- Comment: The text content of the comment