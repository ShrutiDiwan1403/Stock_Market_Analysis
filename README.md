# Stock_Market_Analysis
**Objective Summary**: Stock Price Movement Prediction using Fundamental Analysis 


**Description and Insight**: The investigation delves into the impact of fundamental analysis on the movement of stock market data. A list of machine learning algorithms used and compared to discover the best method for the feature selection are the Chi-squared method, Principal Component Analysis (PCA), Logistic Regression, LightGBM Model, XGBoost Model, Genetic Algorithm, Select K Best Method, Lasso Method, Tree based model, and Cuckoo Search Optimization. The number of features retained is 75 out of 220, with an accuracy of 99.90% for the LightGBM model. Finally, I performed Hyperparameter tuning on the data before diagramming its data flows. In the realm of fundamental analysis, the CatBoost model demonstrated a peak accuracy of 99.80% following k-fold cross-validation, surpassing the performance of the Random Forest Model, Support Vector Classification, and Multi-Layer Perceptron.

![feature_selection_](https://github.com/user-attachments/assets/96e65c53-f0af-44e1-9d6d-16c343e78b7b)


![comparison of training_model](https://github.com/user-attachments/assets/c5817f3d-4e19-41db-a873-471ba1c066ed)


**Programming Language**: Python


**Tool**: Google Colab 


**Glimpse of exploratory analysis:**
The dataset initially comprises 225 financial indicators of US Stocks. The recorded stock data is from 2014 to 2018. Five features were utterly discarded from the dataset before the feature selection process. 

![count_of_each_sector](https://github.com/user-attachments/assets/77080f25-9641-4915-88b9-52d193f97660)

As exhibited in Fig. 2, the highest oscillation was witnessed in the Industrial sector stock. Some companies had a maximum positive gain of close to 200. On the other hand, the most movement of the stock in the negative direction was 100. Glancing at the graph, one can presume that only a handful of businesses in the industrial sector are trading at relatively small amounts. 

![stock_image1](https://github.com/user-attachments/assets/d24f986f-3823-400f-bc45-0e4f677c7f1a)

Fig. 3 also portrays flux in the price variation of the stock. The technology business sector comprises a couple of blue-chip stocks. The highest gain noted was approximately 1200. According to the 2016 technology graph, the technology industry does not have numerous bear 
markets.

![technology graph](https://github.com/user-attachments/assets/2f421bbb-46ba-4466-9676-f85570821314)


**Performance Outcome**:  The study proved that a KNN imputation technique is the most reasonable when dealing with missing values in the dataset (comprising mostly numerical fields). It is best to apply imputation based on industry/sector. LightGBM is the most appropriate algorithm for feature selection. The price direction movement is accurately predicted using the CatBoost algorithm. The model tries to overfit when Random Forest Classifier is used to foretell the direction ( 1 means in upwards order and 0 means in downward order). No sample set was found where the price variation value remained unchanged. No price variation doesn't imply the stock value is 0. The value of the share cannot go below 0. If the value of the share for some reason becomes 0 or falls below the expected threshold value, then the share is delisted. 

![stock__](https://github.com/user-attachments/assets/becb714a-f812-4666-bbe6-3f96cced621a)

