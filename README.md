CAPSTONE PROJECT - 1 
DATA PRE-PROCESSING/ FEATURE ENGINEERING & EXPLORATORY DATA ANALYSIS (EDA) 
§ You are working as a Data Analyst in a Healthcare Analytics Company that partners with hospitals. 
§ The medical team has shared raw cancer patient data (2015-2024) collected from multiple countries. 
§ However, the dataset: 
§ Contains missing values 
§ Has inconsistent formats 
§ Is not analysis-ready 
§ Before using this data for predictive modeling or policy decisions, your task is to clean, preprocess, and analyze the data to extract meaningful 
insights. 
§ After this capstone create a GitHub repository for this and add it to your resume as: 
“Performed end-to-end Data Pre-Processing and Exploratory Data Analysis on a 50,000-record global cancer dataset to identify severity, survival, and cost 
patterns.” 
*********** 
Download the Dataset: https://drive.google.com/file/d/1ldwi4LuV2avz4SNWgfSEnA_W_PwwgtJp/view?usp=share_link 
Dataset Description: This dataset contains global cancer patient data reported from 2015 to 2024, designed to simulate the key factors influencing cancer diagnosis, 
treatment, and survival. It includes a variety of features that are commonly studied in the medical field, such as age, gender, cancer type, environmental factors, and 
lifestyle behaviors.  
§ The dataset is perfect for: 
§ Exploratory Data Analysis (EDA) and for Data Visualization (insightful graphs) 
§ Perform the following tasks 
CAPSTONE PROJECT - 1 
DATA PRE-PROCESSING/ FEATURE ENGINEERING & EXPLORATORY DATA ANALYSIS (EDA) 
 
Tasks: 
Phase Name What to do? Methods / Techniques to Use Questions to Solve 
Data 
Understanding 
Understand dataset 
purpose and target 
variable 
Dataset description reading Identify all columns (Features in the Dataset). 
What does Target_Severity_Score represent?  
Data Inspection Load dataset and check 
structure and quality info(), describe(), isnull().sum() Which columns have missing values? 
What are the descriptive statistics of numerical columns? 
Data Cleaning 
Handle missing values, fix 
data types, remove 
duplicates 
fillna(), astype(), duplicated(), 
drop_duplicates() 
How should missing values in Age, Genetic_Risk, Cancer_Stage be handled?  
Are Patient_IDs duplicated? 
Outlier Handling Detect and treat outliers 
in key numerical columns Boxplot Are there outliers in Treatment_Cost_USD, Survival_Years, 
Target_Severity_Score? 
Encoding 
Categorical 
Variables 
Encode categorical 
features 
Integer Encoding, One-Hot 
Encoding (get_dummies()) 
Should Cancer_Stage use Integer Encoding?  
Should Gender and Cancer_Type use One-Hot Encoding? 
Feature Scaling Scale numerical features StandardScaler, MinMaxScaler Should Age and risk factors use Standard Scaling?  
Should Treatment_Cost_USD use Min-Max Scaling? 
Univariate EDA Analyze individual 
features Histogram, Boxplot, Countplot What is the distribution of Age and Target_Severity_Score?  
Which Cancer_Type is most common? 
Bivariate & 
Multivariate EDA 
Analyze relationships and 
correlations 
Scatter plot, Boxplot, Heatmap, 
corr() 
How does Cancer_Stage affect Survival_Years?  
Which features correlate with severity? 
Insights & 
Conclusion 
Summarize insights and 
give recommendations EDA visuals, summary bullets What are the top 8 insights from the data? 
Which columns influence severity and survival?
