# Guide for Data Science Projects in 2023
This repository explains on defining a problem statement and performing necessary tasks to provide meaningful results.
A walkthrough on a structured approach to ensure a successful completion of a data science project.

# How to start?

**Find/Define a problem statement**:
The problem statement is a critical first step in any data science project, providing a clear definition of the problem to be solved and guiding the development of research questions and hypotheses to reach a well-defined solution.

**How to find the scope of the problem, and where to begin?**
One approach I personally use to start and solve any case scenario is to use the below method and structure a solution accordingly.
![image](https://user-images.githubusercontent.com/40434495/236561740-3a14afbc-97e7-430d-9804-5a11f6f0d1dc.png)

- [x] **Clarify**:
- Define the scope of the problem
- [x] **Constrain**:
-  Refine the problem by setting boundaries and parameters
- [x]**Plan**:
-  Frame your response
-  Data Gathering solutions
-  Collaboration solutions if needed
-  Find the various Statistical analysis that would be implemented
- [x] **Method**:
-  Data Quality Inspection and EDA
-  Data Pre-processing and Feature Engineering (**_Data Cleaning, Data Integration, Data Reduction, Data Transformation & Data Reduction_**)
-  Feature Selection Methodologies 
-  Model Selection & Creation
-  Model Evaluation and Hyper Parameter Tuning
-  Result Visualization
-  Model Deployment
- [x] **Conclude**:
-  Provide a conclusion by explaining the problem statement’s significance and decisions to be taken based on the results


# **Steps involved in solving a Data Science problem**
##  Data science workflow
<p align="center">
  <a href="https://www.python.org/downloads/">
    <img src="https://github.com/shreeramgs/Data-Science-projects/assets/40434495/816ff17b-5f18-42e1-af9f-9661397797c7" alt="Python Logo" width="550">
  </a>
</p>

-   #    Data Analysis
    >   **Data Acquisition**:
    -   Gather requirements
    -   identify relevant data, using APIs, web scraping, flat files or other means of data collection

    >   **Data Quality measures**:
    -   Accuracy
    -   Completeness
    -   Consistency and timeliness
    -   Interpretable/ Believability

    >   **Data Cleaning**:
    -   handling missing values, outliers,inconsistencies
    -   smoothing noisy data
    -   **Tools**: _Python (Pandas, Numpy), Informatica, Talend_

    >   **Data Integration**:
    -   Provide data models explaining heterogeneity and structure of data
    -   Find redundancies
    -   Solve naming inconsistencies from data sources
    -   Find corelation of attributes
    -   **Tools**:  _Talend, Informatica, Oracle_

    >   **Data Reduction**:
    -   **Dimensionality reduction**:
        -   D.W.T
        -   P.C.A
        -   Attribute subset selection
    -   **Numerosity reduction**:
        -   Parametric: regression or log-linear
        -   Non-parametric: _Histograms, clusters, sampling, data aggregation_
    
    >   **Data Transformation**:
    -   Smoothing data
    -   Normalization(_min-max, Z-score, Decimal Scaling_)
    -   Discretization
    -   Conceptual Hierarchy

    >   **Data Visualization**:
    -   **Python**: _Matplotlib and Seaborn _
    -   **R**:  _ggplot2, Plotly, Shiny, tidyquant_
    -   **Tools**:  _Tableau, PowerBI, Google Charts,Qlik_
-   #    Hypothesis Formulation and Testing:
    -   Evaluating mutual exclusive statements on a population of data by using a sample dataset

        >   **Data Sampling**:
        -   **Non probabilistic**
            -   Convenience
            -   Quota
            -   Snowball
            
        -   **Probabilistic**:
            -   Simple Random
            -   Clustered
            -   Stratified

        >   **Make initial assumptions**:
        -   Null Hypothesis (_H0_)
        -   Alternate Hypothesis (_H1_)
        >   **Decide significance levels**
        -   Critical Value and Critical region
        -   One-Tailed Test
        -   Left/Right Tailed Test
        -   Two-Tailed Test

        > **Calculate test statistic**:
        -   Hypothesis test
        -   p value evaluations (_high/low_)
        -   T test
        -   Anova test
        -   Z test  

        >   Gather all evidences and determine to reject/ not reject the null hypothesis

-   #    Feature Engineering:
    -   Perform appropriate data Analysis as mentioned above to get a meaningful set of attributes

-   #    Feature Selection:
    >   **Supervised feature selection**:
    -   **Filter methods**
        -    missing value and information gain
        -   Chi-squared
        -   Fisher's score
        -   correlation coefficient
        -   Variance threshold
        -   Mean Absolute Difference
        -   Dispersion ratio
        -   Spearman's Rho
        -   F score
    -   **Wrapper methods**
        -   Forward selection
        -   Backward selection
        -   Recursive feature elimination
        -   Embedded methods
            -   L1,L2 Regularization
            -   Random forest importance

    >   **Unsupervised feature selection**:
    -   Principal Component Analysis (_**PCA**_)
    -   **Clustering**-based Methods
        -   K means
        -   Hierarchical clustering
        -   Gaussian Mixture models
    -   **Autoencoders**

-   #    Model Creation and Evaluation:   
    -   Now that the redundant or irrelevant features are removed, next step would be to select an appropriate using the selected features
    >   **Split the data**
    -   Train/ Test/ Validation
    -   Stratified Split
    -   Cross-Validation
    -   Stratified K-Fold CV
    -   ShuffleSplit and Stratified Shuffle Split

    >   **Model selection**
    -   Choose appropriate model based on the problem statement
    -   **Linear Models (_Supervised learning models_)**
        -   Linear regression
        -   Logistic regression
        -   Ridge regression
        -   Lasso regression
    -   **Tree-based models (_Supervised learning models_)**
        -   Decision Tree models
        -   Random Forest models
        -   Gradient Boosting Regression
        -   XGBoost
        -   LightGBM Regressor
    -   **Clustering models (_Unsupervised learning models_)**
        -   K means
        -   Hierarchical clustering
        -   Gaussian Mixture models
    
    >   **Model evaluation metrics**
    -   Confusion Matrix
    -   Accuracy, Precision, Recall and F1 Score
    -   ROC and AUC curve 
    -   Gain and Lift 
    -   Confidence Interval
    -   Chi Square
    -   Gini Coefficient
    -   Root Mean Square Error (_RMSE_), Mean Absolute Error (_MAE_), 
    -   Cross Validation (_Leave-p out, k-fold, Holdout, Leave one out)_
    -   Predictive Power

    >   **Hyper-parameter Tuning**
    -   To yield an optimal model with best set of **Hyper parameters** for optimal results

        >   **Traditional methods**
        -   GridSearchCV
        -   RandomizedSearchCV

        >   **Advanced methods**
        -   Bayesian
        -   Early Stopping
        -   Evolutionary
        -   Optuna
        -   Sampling
        -   Pruning
        -   Genetic Algorithms

-   #    **Model Deployment**:
    -   Once the trained model is ready, deploy it for corresponding use case scenarios. Further monitor the model and retrain it respectively
    >   **Local deployment**
    -   Locally used on machine or server. Can also be accessed using frameworks such as:
        -   Streamlit
        -   Django
        -   Flash
        -   Express.JS

    >   **Cloud deployment**
    -   Amazon Web Services (_AWS_)
    -   Google Cloud Platform (_GCP_)
    -   Microsoft Azure

    >   **Containerization**
    -   Docker
    -   Kubernetes

    >   **Using API's**
    -   Frameworks like _Flask, Express.JS, FastAPI_




# Prerequisite needed to solve problems:
Below are few prerequisites that I personally consider to be very useful to solve a use case scenario.

## 1. Python Programming Language
<p align="left">
  <a href="https://www.python.org/downloads/">
    <img src="https://user-images.githubusercontent.com/20041231/211717885-0b1e049b-f5b3-457d-ba7a-9345ec3aa39c.png" alt="Python Logo" width="250">
  </a>
</p>

## 2. Statistics
<p align="left">
  <a href="https://www.sas.com/en_us/software/how-to-buy.html?utm_source=google&utm_medium=cpc&utm_campaign=ana-gen-gbc-dyk-global">
    <img src="https://user-images.githubusercontent.com/20041231/211717931-134aaac2-a8fc-445b-93a6-ae241c66ba5b.png" alt="Python Logo" width="250">
  </a>
</p>

## 3. Databases
<p align="left">
  <a href="https://www.mysql.com/products/workbench/">
    <img src="https://user-images.githubusercontent.com/20041231/211718051-2af3c5ba-cb6d-451b-85ea-5bb01abd9869.png" alt="Python Logo" width="125">
  </a>
    <a href="link_to_your_page">
    <img src="https://user-images.githubusercontent.com/20041231/211718010-30412d4c-9cea-4ae7-858e-a761d0240812.png" alt="Python Logo" width="125">
  </a>
</p>

## 4. Visualization tools
<p align="left">
  <a href="https://www.tableau.com/">
    <img src="https://user-images.githubusercontent.com/40434495/236576283-5bd8858d-263d-48a6-98be-6eb7c7d27a39.png" alt="Python Logo" width="250">
  </a>
</p>

## References
>   Textbooks:
-   Introduction to Algorithms for Data Mining and Machine Learning(Xin-She Yang)
-   Introduction to Statistical Learning
-   Making Sense of Data II: A Practical Guide to Data Visualization, Advanced Data Mining Methods, and Applications
-   DATA SCIENCE INTERVIEW GUIDE ACE-PREP

>   Coursework / Tutorials:
-   [Rachael Hageman Blair](https://publichealth.buffalo.edu/biostatistics/faculty-and-staff/faculty-directory/hageman.html)
-   [Krish Naik](https://www.youtube.com/@krishnaik06)
-   [Analytics Vidhya](https://www.youtube.com/@Analyticsvidhya)