# Drug Review Analysis

<div align="center">
  <a href="https://isel.pt" target="_blank">
    <img src="./img/01_ISEL-Logotipo-RGB_Horizontal.png" alt="ISEL logo" width="400">
  </a>
  <h3 align="center">Exploratory Data Analysis: Drug Review Analysis</h3>
</div>

## Description

This repository contains a comprehensive analysis of drug review data using natural language processing and sentiment analysis techniques. The project is divided into three Jupyter notebooks that handle different aspects of the analysis workflow:

- Exploratory Data Analysis
- Cleaning and Preprocessing
- Sentiment Classification

## Data Source

The data used in this project is sourced from:
- "UCI ML Drug Review dataset" - J. Li, "Kuc hackathon winter 2018 dataset," Kaggle, 2018.

The CSV files are included in the repository and should be placed in the designated directory as shown in the notebook file paths.

## Prerequisites

### System Requirements
- Python 3.8 or later
- Jupyter Notebook or JupyterLab

### Required Libraries
Install the following Python libraries:

```bash
pip install pandas numpy matplotlib nltk textblob
```

### NLTK Resources
Download the necessary NLTK resources:

```python
import nltk
nltk.download('punkt')               # For tokenizing text
nltk.download('averaged_perceptron_tagger')  # For part-of-speech tagging
nltk.download('wordnet')             # For lemmatization
nltk.download('stopwords')           # For filtering out common stopwords
nltk.download('vader_lexicon')       # For VADER sentiment analysis
```

### Plot Configuration
For better visualizations, set the plot style:

```python
import matplotlib.pyplot as plt
plt.style.use('ggplot')
```

## Getting Started

1. Clone this repository
2. Install the required libraries
3. Download the necessary NLTK resources
4. Run Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## Notebooks

### 1. Data Visualization (`data-visualisation.ipynb`)
This notebook performs exploratory data analysis (EDA) on the drug review dataset to understand:
- Distribution of reviews across different drugs
- Rating patterns
- Review length analysis
- Temporal trends in drug reviews

### 2. Data Cleaning and Pre-processing (`data-cleaning-and-pre-processing.ipynb`)
This notebook focuses on preparing the raw data for analysis by:
- Cleaning text data
- Handling missing values
- Removing unnecessary columns
- Implementing text normalization techniques (tokenization, lemmatization, etc.)

### 3. Review Sentiment Classification (`review-sentiment-classification.ipynb`)
This notebook applies sentiment analysis techniques to classify the polarity of drug reviews:
- Using TextBlob for basic sentiment analysis
- Implementing VADER sentiment analysis for more nuanced results
- Visualizing sentiment distribution across different drugs
- Comparing sentiment metrics with user ratings

## Limitations

- This is a proof of concept and should not replace professional medical advice
- Recommendations are limited by the quality and quantity of the training data
- The system does not account for individual patient factors such as age, gender, or medical history

## Acknowledgments

Developed by Ana Sofia Pinto as part of the DrugDRecSys-SUSA dissertation.

## License

[MIT License](LICENSE)