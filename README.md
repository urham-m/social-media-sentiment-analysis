# Sentiment Analysis of Airline Tweets

This project finds out how people feel about airlines on Twitter. It cleans the tweets (tokenizing, removing stop words and lemmatizing with NLTK), labels them with the pre-trained VADER model, and trains a Logistic Regression classifier that reaches about 80% accuracy. It then shows sentiment trends over time, by airline and by user timezone, and makes word clouds and charts to show what customers like and complain about.

## How to run

1. Clone the repo and go into the folder:
```
   git clone https://github.com/urham-m/airline-sentiment-analysis.git
   cd airline-sentiment-analysis
```
2. Create a virtual environment and install the requirements:
```
   python -m venv .venv
   .venv\Scripts\activate
   pip install -r requirements.txt
```
   (On Mac/Linux use `source .venv/bin/activate` instead.)
3. Open `sentiment_analysis.ipynb` in Jupyter or VS Code, select the **`.venv` (Python)** kernel, then run the cells from top to bottom. The first run downloads a few small NLTK files, so you need internet once.
4. Charts, word clouds and the labeled tweets are saved in the `outputs/` folder.

## Dataset source

https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment
