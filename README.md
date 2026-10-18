# Sentiment Analysis

This project explores sentiment classification for text reviews using natural language processing (NLP) and machine learning. It focuses on identifying whether a given review is positive, negative, or neutral, and compares several classifier models trained on a movie-review dataset.

## Project overview

The workflow in this project includes:

- Loading and preprocessing text data
- Normalizing case and expanding contractions
- Tokenizing and cleaning review text
- Applying stemming or lemmatization
- Converting text to numerical features with TF-IDF
- Training multiple classification models to compare performance
- Evaluating the models using accuracy and confusion-matrix metrics

The notebook and supporting utilities are designed for experimentation and learning, with an emphasis on preprocessing quality and model comparison.

## Files in this project

- `SentimentAnalysis.ipynb` — main notebook containing the full data exploration, preprocessing, model training, and evaluation steps
- `nlp_utils.py` — helper functions for text normalization, tokenization, stemming, and lemmatization
- `contractions.py` — contraction expansion utilities
- `TextAnalytics.txt` — text review dataset used for model training
- `requirements.txt` — Python dependencies for the project
- `sent/` — local virtual environment used in this workspace

## Tech stack

- Python 3.12
- NLTK
- scikit-learn
- pandas
- NumPy
- Matplotlib / Seaborn / WordCloud

## Setup

From the project directory:

```bash
python -m venv sent
```

On Windows PowerShell:

```powershell
cd "C:\Users\Macks\OneDrive\Desktop\portfolio project\Sentiment Analysis"
.\sent\Scripts\Activate.ps1
pip install -r requirements.txt
```

If you see missing NLTK resources, download them in Python:

```python
import nltk
nltk.download("stopwords")
nltk.download("punkt")
nltk.download("wordnet")
nltk.download("omw-1.4")
nltk.download("averaged_perceptron_tagger")
```

## Running the project

1. Open `SentimentAnalysis.ipynb` in Jupyter or VS Code.
2. Run the cells in order to:
   - load the dataset,
   - preprocess the text,
   - train the classifiers,
   - compare results.

The notebook includes experiments with models such as:

- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

## Dataset notes

The dataset is stored in `TextAnalytics.txt` and contains movie reviews with labels represented in a text format similar to review text files used in sentiment-analysis tutorials. The project converts the text into a training corpus for classification.

## Example use cases

This project can be adapted for:

- sentiment classification of product reviews,
- social media opinion analysis,
- feedback categorization,
- text classification experiments in NLP.

## License

This project is intended for educational and portfolio use. If you plan to reuse it or distribute it publicly, check whether the dataset or code requires a specific license.
