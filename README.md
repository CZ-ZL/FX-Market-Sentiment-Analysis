### **Applying Sentiment Analysis to Brazilian Portuguese Financial News to Enhance Trading Decisions within the Foreign Exchange (FX) Market**

Current Task: Plan

### 5-Step Sentiment Analysis Process (Can Vary)

1. Create Testable Hypothesis
    1. Let the hypothesis drive the topics of textual data you work with (relevance)
2. Extract Relevant Textual Data (called a ‘corpus’: textual data)
    1. In the case of macroeconomic conditions: large file of news articles is helpful to train a model on (aggregate data)
3. Clean Relevant Textual Data
    1. GIGO - “Garbage In, Garbage Out” - bad data, bad output
4. Estimate Sentiment Measure
    1. Quantify the sentiment (Postive, Negative, Neutral) for the *aggregate economy*
5. Test / Validate the hypothesis

**Potential Models for Financial Portuguese Sentiment Analysis**

- MeaningCloud: https://www.meaningcloud.com/developer/sentiment-analysis
    - Input text, outputs detailed JSON of text sentiment features
- ELG: https://live.european-language-grid.eu/catalogue/tool-service/477
- FinBERT-PT-BR: https://huggingface.co/lucas-leme/FinBERT-PT-BR
    - pre-trained NLP model to analyze sentiment of Brazilian Portuguese financial texts
- Pysentimiento: https://huggingface.co/pysentimiento/bertweet-pt-sentiment
    - **Base Paper:** https://arxiv.org/pdf/2106.09462
    - Repository: https://github.com/pysentimiento/pysentimiento/
- mkuchak: https://github.com/mkuchak/sentiment-analysis
    - a simple, complete, application with back-end/front-end for an AI model that analyzes/predicts the sentiment of a text written in Brazilian Portuguese

**Resources for Sentiment Analysis on Financaial News**

- https://www.dowjones.com/professional/resources/blog/a-primer-for-sentiment-analysis-of-financial-news

***Three Categories:***
- Good for the Brazilian Real
- Good for the US Dollar
- Good for Neither

**Factors favorable to the USD:**
- Increases in internal interest rates: Considering that **USA is the safest economy in the world**, when the **Federal Reserve raises the prime rate**, the US$ tends to appreciate because higher interest rates attracts foreign capital, increasing the US$ demand and appreciating the currency.
- Economic Indicators: Raising indicators such as GDP growth (increase in consumption) , increasing job creation, decreasing unemployment, payroll, low inflation, real state market, surplus in trade balance, increasing demand for treasury bonds
- In a volatile world, money flies to quality, going massively to USA.

**Factors favorable to the Brazilian currency – REAL – R$**
- Higher Brazilian Interest Rates, attracts external investments, appreciating the local currency
- Increasing in commodities prices such as soybean, corn, coffee, iron ore. When these prices raise, a surplus in trade balance appreciates REAL
- Increasing in foreign investment in Brazil’s infrastructure
- Political stability
- Controlled inflation and fiscal policies

**9/18**

News

- FOMC decision (USA)
- COPOM decision (Brasil)

Possibile Outcomes:

1. FOMC and COPOM cut interest rates: Good for R$
2. FOMC cuts and COPOM keeps interest rates unchanged: Good for R$
3. FOMC and COPOM keeps interest rates unchanged: Neutral for R$
Result - 4. FOMC cuts and COPOM raises: Bad for R$ 

**Why do I not translate the articles to English, and then run the pipeline?**
Perform sentiment analysis directly on articles in Brazilian Portuguese (PT-BR). Why:
1. **Context and Nuance**: Sentiment is contextual and language-specific - necessary for accurate sentiment assessment.
2. **Model Performance**: My model is trained on PT-BR news articles
3. **Translation Errors**: Translations may include errors; variations can significantly affect trading signals.
4. **Domain-Specific Vocabulary**: News articles have specialized vocabulary. Models designed for PT-BR will understand the terms in context.
