# NHS-Hospital-Waiting-Times-Prediction
Project Overview
The goal of this project is to analyze historical NHS waiting time data to predict future waiting times for emergency departments in the top 15 NHS hospitals. These predictions are crucial for hospital administrators to manage patient flow, optimize resource allocation, and ultimately improve patient care.

Data
The dataset used in this analysis includes historical waiting time data from NHS hospitals. The data was collected from the NHS Emergency Department performance reports and merged into a single dataset.

Data Structure
Period: The time period for the data (monthly).
Org Code: The unique code for each NHS organization.
Org Name: The name of the NHS hospital or trust.
Various Attendance and Waiting Time Metrics: Includes metrics such as "Attendances over 4hrs Type 1," "Attendances over 4hrs Type 2," and more.
Methodology
Exploratory Data Analysis (EDA)
Initial data exploration involved examining the distribution of waiting times across different hospitals, identifying trends, and visualizing the data to understand the underlying patterns.

Feature Engineering
Features were created by combining and aggregating different attendance metrics. The total attendance and waiting times over 4 hours were key features used in the predictive modeling.

Machine Learning Models
Random Forest: Used as a baseline model to predict future waiting times based on historical data.
XGBoost: Implemented for enhanced predictive accuracy. The model was fine-tuned using grid search to identify the optimal parameters.
Future Predictions
The project also includes a forecasting component, where future waiting times for the next three months were predicted using the ARIMA model, providing actionable insights for hospital administrators.

Results
Random Forest: The model achieved a mean absolute error of approximately 3256.78 and an R^2 score of 0.697.
XGBoost: After hyperparameter tuning, the model achieved a mean absolute error of 3846.60 and an R^2 score of 0.991.
Conclusion
This analysis provides valuable insights into NHS hospital waiting times and helps in proactive planning to manage patient flow. The predictions suggest that without significant intervention, some hospitals may continue to experience high waiting times, highlighting the need for strategic improvements.

Future Work
Incorporating additional features such as hospital capacity and staffing levels.
Exploring advanced machine learning models like Neural Networks.
Implementing real-time predictions for dynamic hospital management.
Expanding the dataset to include more hospitals and a longer historical period.
