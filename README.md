E-Commerce Churn Analytics: Distributed ML Pipeline
Overview
An end-to-end distributed machine learning pipeline designed to predict dynamic customer churn in a large-scale e-commerce environment. Processing a massive clickstream dataset of over 109 million events, this project leverages PySpark for heavy-duty data engineering and behavioral clustering, ultimately deploying high-performance gradient boosting models to accurately identify at-risk revenue.  
Key Technical Achievements
Big Data Processing Pipeline: Engineered a robust PySpark pipeline to clean and process 109M+ raw events, implementing a strict temporal train/label split to guarantee zero data leakage during model training.  
Dynamic Customer Profiling: Computed Length-Recency-Frequency-Monetary (LRFM) profiles for 347,000+ distinct users. Utilized distributed K-Means Clustering—optimizing the k value via Silhouette Score—to establish accurate, 3-class dynamic churn labels.  
Advanced Feature Engineering: Extracted 14 nuanced behavioral features and resolved severe class imbalances using SMOTE, successfully synthesizing and scaling the minority class from 274,000 to 793,000 records.  
Rigorous Model Benchmarking: Systematically evaluated 7 distinct classifiers: XGBoost, LightGBM, Random Forest, CatBoost, SVM, KNN, and a custom Soft Voting Ensemble.  
Results & Business Impact
Peak Performance: The LightGBM architecture achieved top-tier predictive performance with a 95.0% test accuracy.  
Actionable Intelligence: Translated the raw predictive metrics into a comprehensive business report, successfully identifying $81.7M in revenue at risk due to potential churn.  
Tech StackCore Languages: Python   Big Data & Processing: PySpark (v4.0.2)   Machine Learning & Modeling: LightGBM, XGBoost, CatBoost, Scikit-Learn (Random Forest, SVM, KNN), Imbalanced-learn (SMOTE) 
