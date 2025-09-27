# Sentiment Analysis of Solo Leveling Game Reviews on Google Play Store

## 📌 Project Overview
This project analyzes user reviews of the **Solo Leveling** mobile game from Google Play Store using **AI (IBM Granite Models)**.  
The main objective is to explore sentiment distribution, extract key insights from user feedback, and provide recommendations that can help developers improve the overall gaming experience.  

The analysis follows these steps:  
1. Data collection through web scraping of Google Play Store reviews.  
2. Preprocessing the text data (cleaning, casefolding, tokenizing, stopword removal, stemming).  
3. Sentiment analysis using **IBM Granite Models**.  
4. Visualization of sentiment distribution and extraction of dominant keywords.  
5. Generating insights and actionable recommendations.  

---

## 📂 Raw Dataset
The dataset used for this analysis is scraped from **Google Play Store reviews** for the *Solo Leveling* game.  
- [Link to dataset (https://drive.google.com/file/d/1db1U6G26FjpCKBy8ES0bWeUCj5Uj2GMk/view?usp=sharing)

---

## 🔍 Insights & Findings
- **Sentiment Distribution**: Majority of reviews are **Positive: ~49.34%'**, followed by **Negative: ~38.73%**, and **Neutral: ~11.92%**.  
- **Positive Reviews** highlight strengths in **'nya' (732 occurrences), 'bug' (664 occurrences), 'game' (638 occurrences), 'loading' (627 occurrences), and 'bagus' (503 occurrences)**.  
- **Negative Reviews** mostly mention **'game' (2492 occurrences), 'bug' (2351 occurrences), 'loading' (1931 occurrences), 'nya' (1744 occurrences), and 'Game' (972 occurrences)**.  
- **Trend Analysis** Inconclusive Trend suggests no consistent pattern in user satisfaction over time, with sentiments merely fluctuating without a clear upward or downward trajectory, necessitating a larger dataset and advanced NLP for reliable conclusions.  

**Key Insights:** Many users report bugs, such as loading issues and tutorial disappearances.Performance problems are frequently mentioned, including high RAM usage and slow loading times. The game's size is a concern for some users, with complaints about its large storage requirement  

---

## 🤖 AI Support Explanation
The analysis is powered by **IBM Granite Models**, which provide:  
- **Sentiment Classification** → Automatically categorizes reviews into positive, negative, and neutral.  
- **Keyword Extraction** → Identifies frequent terms associated with each sentiment type.  
- **Trend Analysis** → Highlights changes in sentiment over time.  
- **Insight Generation** → Summarizes findings and assists in producing actionable recommendations.  

Example prompts used with Granite:  
```python
agent.invoke({"input": "analyze the sentiment distribution in the dataset (positive, neutral, negative)"})
agent.invoke({"input": "create a sentiment graph of review data showing the proportion of positive, negative, and neutral reviews"})
agent.invoke({"input": "extract the top keywords mentioned in negative reviews"})
agent.invoke({"input": "summarize key insights and recommendations based on the sentiment analysis"})
