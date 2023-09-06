# Financial-Sentiment-Analysis

![chris-liverani-NDfqqq_7QWM-unsplash](https://github.com/aswinram1997/Financial-Sentiment-Analysis/assets/102771069/cef474d3-bf3d-4e0f-accf-47b898fe1a60)

## Project Overview
In today's data-driven financial landscape, the development of a Financial Sentiment Analysis Model is of paramount importance. This model harnesses natural language processing and machine learning techniques to systematically evaluate sentiment in financial data, offering invaluable insights for investment decisions, risk management, and market forecasting. By quantifying sentiments expressed in various financial sources, this model not only addresses the growing demand for sophisticated data analysis tools but also paves the way for innovative applications that can enhance decision-making processes across the financial industry, promising a more informed and competitive future. Therefore, this project's objective is to develop a Financial Sentiment Analysis Model that can predict the sentiment of financial markets and assets accurately, enabling investors, traders, and financial professionals to make more informed decisions and navigate the complexities of the ever-evolving financial landscape with greater confidence.

## Dataset Overview
The [Kaggle Dataset](<https://www.kaggle.com/datasets/sbhatti/financial-sentiment-analysis>) consists of 5836 rows and 2 columns (Sentence, Sentiment). The "Sentence" column contains short text data related to the financial market. The "Sentiment" column provides labels indicating the sentiment expressed in each sentence, which can be categorized as positive, negative, or neutral sentiments, making it a valuable resource for sentiment analysis in the context of financial markets.

## Methodology
- Data Collection: Gathered data from the provided Kaggle dataset, which includes financial sentences labeled with sentiment. This dataset was curated with sentiment labels, thereby constituting a foundational corpus for sentiment analysis.

- Data Splitting: Split the dataset into training and testing sets to assess model performance.

- Exploratory Data Analysis: Conducted exploratory data analysis to gain insights into the dataset's characteristics, distribution of sentiments, and potential patterns.

- Text Preprocessing and Model Training
    - A. Text Blob
    
        The initial phase of model development commenced with the implementation of a rule-based approach utilizing Text Blob. This rudimentary model served as a foundational reference point to assess sentiment analysis on financial textual data.
    
    - B. Machine Learning Models with TF-IDF
         
         Multinomial Naive Bayes: Multinomial Naive Bayes, in conjunction with TF-IDF vectorization, was harnessed to categorize financial sentences into sentiment categories. The performance of this model was methodically evaluated to ascertain its suitability for sentiment analysis in the financial domain.
         
         Random Forest: The project also explored the utility of Random Forest, a prominent ensemble learning algorithm, in tandem with TF-IDF vectorization. This exploration sought to discern the predictive potential of ensemble models in the context of sentiment analysis for financial text data.

    - C. Long-short term memory (LSTM) with Word2Vec
    
        Venturing into the domain of deep learning, the research culminated in the development of an LSTM (Long Short-Term Memory) model, a type of recurrent neural network (RNN). This model was constructed using Word2Vec embeddings, thereby imbuing it with the capacity to grasp nuanced semantic nuances. The deployment of deep learning techniques aimed to elevate the accuracy and context-awareness of the sentiment analysis process in the financial domain.

## Results
In this sentiment analysis project, we experimented with four models: Text Blob (baseline model), Multinomial Naive Bayes with TF-IDF, Random Forest with TF-IDF, and LSTM with Word2Vec. Although Multinomial Naive Bayes was more accurate, we favored the Random Forest, which, while a bit less accurate, generalized better. Additionally, the LSTM model, despite being deep learning, only did better than Text Blob, not surpassing Multinomial Naive Bayes or Random Forest. This suggests that deep learning models always doesn't guarantee superior results. In conclusion, Random Forest's strong generalizability makes it the top choice for sentiment prediction. After rigorous experimentation and fine-tuning, the winning model's performance remains satisfactory; thus, future work should focus on collecting a more extensive and diverse dataset for financial market sentiment analysis to bolster model robustness and explore its performance in broader data contexts.

## Conclusion
In the dynamic realm of finance, sentiment analysis models, such as the one crafted in this project, serve as indispensable instruments for facilitating well-informed investment choices, risk mitigation, and the anticipation of market trends. Notably, the Random Forest model emerged as the optimal choice in our experimentation, excelling in both performance and generalization. To augment the model's resilience and broaden its utility, forthcoming initiatives should give precedence to procuring a more extensive and varied dataset for forecasting sentiments in financial markets. Additionally, there is a need to explore alternative combinations of algorithms and word embeddings to advance the model's efficacy.


