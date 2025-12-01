# This repository contains the final project for CS133<hr>

## Our goal:<br>
Does Twitter Sentiment Correlate with Apple Stock data? <br>


We analyze Twitter sentiment about Apple and compare it with the actual Apple stock to see whether social media signals correlate with market movements.

**1. Dataset**<br>
	- Twitter dataset: “apple-twitter-sentiment-texts” from Kaggle (Apple-related tweets with sentiment labels -1/0/1).<br>
    - Twitter dataset(with date): "iphoe14-query-tweets" from Kaggle (From July to Sept 2022).<br>
	- Stock dataset: "apple_stock" from Kaggle.<br>
    - Apple Financial dataset: download from apple website and convert it to csv file to make it as data frame.<br>


**2. Repository Structure**<br>
    - notebooks/source_code/ <br>
	- apple_stock_analysis.ipynb:  stock price cleaning and visualization with ML model<br>
	- word_breaker.ipynb:  text preprocessing and tokenization with ML model<br>
	- apple_consolidated_analysis.ipynb:  iPhone Sales Performance and Market Capitalization Analysis<br>
	- corr_twit_and_stock.ipynb:  correlation analysis between sentiment and stock with ML models<br>
	- requirements.txt: Python dependencies.<br>


**3. Methods<br>**
	- Text preprocessing:<br>
	- Lowercasing, cleaning, tokenization, custom sentiment dictionary from ML coefficients.<br>
	- Machine learning:<br>
	- TF‑IDF<br>
	- Logistic Regression<br>
    - Random Forrest<br>
	- Train/test split with stratification on sentiment labels.<br>
	- Evaluation:<br>
	- Accuracy, precision, recall, F1‑score.<br>
	- Confusion matrix for sentiment classes.<br>


**4. Key Findings<br>**
    - Neutral words dominated Daily Twitter sentiment around Apple, with positive and negative word counts moving together without clear direction changes in stock returns.  <br>
    - Logistic Regression and Random Forest models using technical indicators achieved only modest accuracy (≈0.46–0.53), and adding sentiment features did not materially improve prediction performance.  <br>
    - Random Forest feature importance showed that traditional market features (MA5, MA20, MACD, RSI, returns) explained most of the variation in quarterly stock moves, while the sentiment score contributed the least.  <br>
    - Gap up/down and intraday up/down patterns by weekday and month revealed strong seasonality in 2024 price action, independent of Twitter sentiment levels.  <br>
    - Quarterly revenue, market cap, and stock price for Apple moved closely together, confirming that fundamentals remain strongly correlated with valuation, whereas Twitter sentiment showed only weak correlation with returns.<br>

**5. How to Run <br>**
	1. Clone this repo:<br>
	    - git clone <repo-url> <br>
	2. Create a virtual environment <br>
	3. Install dependencies:<br>
	    - pip install -r requirements.txt <br>
    4. csv files should be in the dataset folder
    5. Open the notebooks

**6. References**
    - Kaggle: 
        apple‑twitter‑sentiment‑texts dataset<br>
        iphone14-query-tweets dataset<br>
        apple_stock dataset<br>    
    - Apple Financial dataset from apple newsroom
	- scikit‑learn documentation for text classification and model evaluation.

