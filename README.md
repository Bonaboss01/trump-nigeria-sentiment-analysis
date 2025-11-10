# trump-nigeria-sentiment-analysis
NLP project analyzing global reactions to Donald Trump’s 2025 statement on Nigeria using sentiment analysis, topic modeling, and named entity recognition.
# 🧠 Trump-Nigeria Sentiment Analysis

**Natural Language Processing (NLP) project analyzing global reactions to Donald Trump’s 2025 statement on Nigeria using sentiment analysis, topic modeling, and named entity recognition.**

---

## 📊 Data Collection

I initially planned to scrape tweets related to Donald Trump’s 2025 statement on Nigeria using the `snscrape` Python library. However, due to recent compatibility issues with Python 3.13, `snscrape` produced import errors that prevented execution.

I explored several alternative approaches, including:

- **Tweepy (Twitter API v2):** Provides live tweet collection but requires a valid API key and is rate-limited for free accounts.  
- **NewsAPI / GDELT:** Could collect related news articles but would shift the project’s focus away from individual opinions to media coverage.  
- **Pre-existing open-source Twitter datasets:** Contained unrelated or outdated topics.

Given that the purpose of this project was to **apply and demonstrate NLP techniques** — not to test API integrations — I opted to generate a **synthetic dataset** that realistically mirrors social media discourse on the topic.

The dataset includes **2,000 samples** across multiple perspectives:
- pro-Trump  
- anti-Trump  
- neutral  
- fact-checking  
- sarcastic  
- sovereignty-defending tweets  

Each record includes realistic metadata such as **timestamps**, **likes**, and **retweets**.

---

### ✅ Advantages of This Approach

- **Reproducibility:** Anyone can run the notebooks without API credentials.  
- **Control:** Balanced sentiment classes and representativeness across perspectives.  
- **Continuity:** Enabled smooth progression to the analytical workflow — text cleaning, sentiment analysis, topic modeling, and named entity recognition.

---

📁 *Dataset:* `data/tweets_raw.csv`  
📒 *Next Steps:* Proceed to text preprocessing in `notebooks/03_text_cleaning_preprocessing.ipynb`.

