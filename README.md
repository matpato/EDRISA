
# Python Projects for Drug Review Analysis

## Description
This repository contains three Jupyter notebooks that handle different aspects of drug review data analysis: Exploratory Data Analysis, Cleaning and Preprocessing, and performing Sentiment classification.

## Data Source
The data files used in these notebooks is sourced from: "UCI ML Drug Review dataset" - J. Li, "Kuc hackathon winter 2018 dataset," Kaggle, 2018. 

These csv files are included in the repository and should be placed in the designated directory as shown in the notebook file paths.

## Prerequisites
- Python 3.8 or later
- Jupyter Notebook or JupyterLab

### Libraries
Install the following Python libraries using pip:

```bash
pip install pandas numpy matplotlib nltk textblob
```

### NLTK Resources
Ensure you have the following NLTK resources downloaded:

```python
import nltk
nltk.download('punkt')  # For tokenizing text
nltk.download('averaged_perceptron_tagger')  # For part-of-speech tagging
nltk.download('wordnet')  # For lemmatization
nltk.download('stopwords')  # Stopwords that can be filtered out in preprocessing
nltk.download('vader_lexicon')  # For VADER sentiment analysis
```

### Additional Setup
Set the style of plots to 'ggplot' for better aesthetics:

```python
import matplotlib.pyplot as plt

plt.style.use('ggplot')
```

## Usage
Open your command line interface and run Jupyter Notebook:

```bash
jupyter notebook
```

## Notebooks

### 1. Data Visualization (`data-visualisation.ipynb`)
This notebook includes various exploratory data analysis (EDA) techniques to visualize different aspects of drug reviews. This notebook begins with an outline of the various exploratory data analysis (EDA) techniques implemented.

### 2. Data Cleaning and Pre-processing (`data-cleaning-and-pre-processing.ipynb`)
This notebook focuses on preparing the raw data for analysis. The notebook starts by detailing its structure focused on data cleaning tasks. It prepares the raw data for analysis by cleaning text data, handling missing values, and removing unnecessary columns.

### 3. Review Sentiment Classification (`review-sentiment-classification.ipynb`)
This notebook outlines its structure at the beginning, focusing on applying sentiment analysis using TextBlob and VADER to classify the polarity of drug reviews. It also includes sections for visualizing the results and comparing different sentiment metrics.

