What Drives Diamond Prices?
A Data-Driven Classification Analysis
This repository contains the materials submitted for my coursework assignment titled “What Drives Diamond Prices? A Data-Driven Classification Analysis” 
Project 2 Report
.
The project investigates how physical and quality-related diamond characteristics influence whether a diamond belongs to a high-price category using statistical and machine learning classification models.
Project Objective
Rather than predicting exact diamond prices, this study focuses on classifying diamonds into high-priced and non-high-priced categories. This approach reflects real-world pricing practices in the diamond industry, where diamonds are often segmented into price tiers for valuation, inventory management, and pricing strategy.
The analysis examines how attributes such as carat, cut, colour, clarity, depth, table, and physical dimensions contribute to price classification outcomes.
Dataset
The dataset consists of 53,794 observations after data cleaning and includes:
Numerical variables: carat, depth, table, x, y, z, price
Categorical variables: cut, colour, clarity
Duplicate observations were removed, and categorical variables were converted to factors prior to modelling to ensure valid statistical inference.
Methodology
The analysis follows a structured data science workflow:
Data cleaning and preprocessing
Exploratory Data Analysis (EDA)
Construction of a binary classification target
Train–test split (70% training, 30% testing)
Model fitting, evaluation, and comparison
A quantile-based threshold was used to define the classification target, with diamonds in the top 25% of the price distribution labelled as High.
Classification Models
The following classification models were implemented and compared:
Logistic Regression
Linear Discriminant Analysis (LDA)
Quadratic Discriminant Analysis (QDA)
k-Nearest Neighbours (KNN)
Neural Network
Model performance was evaluated using test-set classification accuracy and confusion matrices.
Key Findings
Logistic Regression and LDA achieved the highest classification accuracy, indicating strong linear separability in the data.
Size-related variables, particularly carat and physical dimensions, are the strongest drivers of price classification.
More complex models, such as Neural Networks, did not outperform simpler statistical models for this structured dataset.
Model interpretability and alignment with data structure proved more important than model complexity.
Tools and Libraries
The analysis was conducted in R, using key packages including:
tidyverse
MASS
e1071
class
ggplot2
corrplot
nnet
Repository Contents
Project 2 Report.pdf
Final written report containing methodology, results, and interpretation.
R code (Appendix)
Code used for data cleaning, EDA, model training, and evaluation.
README.md
Project overview and documentation.
Notes
This repository is intended for academic submission purposes. All modelling choices and interpretations align with the assignment requirements and marking criteria.
