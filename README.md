# OlaChurn_analysis
Project on OLA Driver Churn Analysis

# Problem Statement
Recruiting and retaining drivers is seen by industry watchers as a tough battle for Ola. Churn among drivers is high and it’s very easy for drivers to stop working for the service on the fly or jump to Uber depending on the rates.

As the companies get bigger, the high churn could become a bigger problem. To find new drivers, Ola is casting a wide net, including people who don’t have cars for jobs. But this acquisition is really costly. Losing drivers frequently impacts the morale of the organization and acquiring new drivers is more expensive than retaining existing ones.

You are working as a data scientist with the Analytics Department of Ola, focused on driver team attrition. You are provided with the monthly information for a segment of drivers for 2019 and 2020 and tasked to predict whether a driver will be leaving the company or not based on their attributes like

Demographics (city, age, gender etc.) Tenure information (joining date, Last Date) Historical data regarding the performance of the driver (Quarterly rating, Monthly business acquired, grade, Income)

# About the data
Column Profiling:

• MMMM-YY : Reporting Date (Monthly) (date-time)

• Age : Age of the employee (numerical)

• Gender : Gender of the employee – Male : 0, Female: 1 (categorical)

• City : City Code of the employee (categorical)

• Education_Level : Education level – 0 for 10+ ,1 for 12+ ,2 for graduate (categorical)

• Income : Monthly average Income of the employee (numerical)

• Date Of Joining : Joining date for the employee (date-time)

• LastWorkingDate : Last date of working for the employee - Target Feature (date-time, but will be converted to categorical)

• Joining Designation : Designation of the employee at the time of joining (categorical, ordinal)

• Grade : Grade of the employee at the time of reporting (categorical, ordinal)

• Total Business Value : The total business value acquired by the employee in a month (negative business indicates cancellation/refund or car EMI adjustments) (numerical)

• Quarterly Rating : Quarterly rating of the employee: 1,2,3,4,5 (categorical, ordinal - higher is better)

# Objectives:
- Identify key factors contributing to driver churn.
- Build predictive models to forecast churn and classify drivers at risk of leaving.
- Provide actionable insights to Ola management to improve driver retention strategies.

# Data Collection:
The project utilizes a comprehensive dataset obtained from Ola's internal databases, containing historical records of driver activities, trip details, earnings, ratings, and other relevant metrics. The dataset covers a significant timeframe to capture trends and patterns in driver behavior.

# Data Preprocessing:
Data preprocessing involves cleaning, formatting, and transforming raw data into a suitable format for analysis. This step includes handling missing values, outlier detection, feature engineering, and encoding categorical variables. Additionally, exploratory data analysis (EDA) techniques are applied to gain initial insights into the data.

# Feature Selection:
Feature selection is crucial for identifying the most influential factors affecting driver churn. Statistical methods, correlation analysis, and domain knowledge are leveraged to select relevant features that contribute to churn prediction models.

# Model Building:
Several machine learning algorithms, such as logistic regression, decision trees, random forests and XGBoost are explored to develop predictive models for driver churn. Hyperparameter tuning and cross-validation techniques are applied to optimize model performance and ensure robustness.

# Evaluation Metrics:
The performance of churn prediction models is evaluated using various metrics, including accuracy, precision, recall, F1-score, ROC AUC score, and confusion matrix. These metrics provide insights into model effectiveness, discrimination ability, and balance between true positives and false positives.

# Conclusion:
- After hyperparameter tuning, the RandomForestClassifier shows improved performance across all metrics compared to the DecisionTreeClassifier.
- It achieves higher accuracy (90.05%) and Cross Validation Score (97.28%), indicating better generalization and robustness.
- The ROC AUC Score (89.51%) is higher, suggesting improved discrimination between classes.
- The F1 Score (Churn) has also increased to 85, indicating better balance between precision and recall for the churn class.
- Overall, the RandomForestClassifier outperforms the DecisionTreeClassifier after hyperparameter tuning, demonstrating higher accuracy, better generalization, and improved performance across multiple metrics. -- - Therefore, the RandomForestClassifier is preferred for this classification task.

# Model Performance:
XGBoost and Random Forest Classifier stands out as the best-performing model overall, with consistently high accuracy across all metrics for both predicting churn and non-churn.
