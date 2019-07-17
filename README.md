# wine-reviews-pyspark

## Wine Review Analysis
To start, register a Databricks Community account to use Spark for free  
https://community.cloud.databricks.com/

Dataset can be downloaded from here:  
https://www.kaggle.com/zynicide/wine-reviews

### Summary of this analysis
1. Data Extraction  
2. Data Exploration & Preprocessing    
    2.1 Remove Null value  
    2.2 Lowercase text value   
    2.3 Country Feature Preprocessing  
    2.4 Grapes Variaty Feature Preprocessing
    
3. Features Extraction  
    3.1 Tokenizor  
    3.2 Stopwords Remover   
    3.3 TF-IDF Text Feature Extraction  
    3.4 Word2Vec Text Feature Extraction   
    3.5 Transform Points as categorical feature with Bucketizer  
    3.6 Transform Country, Taster_name, Variety as categorical features with StringIndexer and OneHotEncoderEstimator  
    3.7 Choose Top-K best features with ChiSqSelector    
    3.8 Create Feature Extraction Pipeline
    
4. Model Exploration  
    4.1 Classification  
    - 4.1.1 Features used
      - TF-IDF Features
      - Word2Vec Features
      - Numerical & Categorical Features
      - Combine Features
      - Selected Features  
      
     - 4.1.2 Models 
        - Logistic Regression
        - Support Vector Machine
        - Random Forest
        - MLPC (MultilayerPerceptronClassifier)

    4.2 Regression
      - Gradient Boosting Regression
      - Random Forest Regression
      - Linear Regression

5. Cross Validation & Hyper-Parameters Tuning  
    5.1 Classification Hyper-Parameters Tuning  
    5.2 Regression Hyper-Parameters Tuning
    
