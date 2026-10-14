# Sentiment Analysis of Airline Tweets

This project finds out how people feel about airlines on Twitter. It cleans the tweets (tokenizing, removing stop words and lemmatizing with NLTK), labels them with the pre-trained VADER model, and trains a Logistic Regression classifier that reaches about 80% accuracy. It then shows sentiment trends over time, by airline and by user timezone, and makes word clouds and charts to show what customers like and complain about.

## How to run

1. Clone the repo and go into the folder:

```
   git clone https://github.com/urham-m/social-media-sentiment-analysis
   cd social-media-sentiment-analysis
```

2. Create a virtual environment and install the requirements:

```
   python -m venv .venv
   .venv\Scripts\activate
   pip install -r requirements.txt
```

(On Mac/Linux use `source .venv/bin/activate` instead.)

3. Open `sentiment_analysis.ipynb` in Jupyter or VS Code, select the **`.venv` (Python)** kernel, and run the cells from top to bottom. The first run downloads the required NLTK data files, so an internet connection is needed.

4. The generated charts, word clouds, and labeled tweets are saved in the `outputs/` folder.

## Dataset source

https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment
