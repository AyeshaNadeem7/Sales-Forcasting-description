# Sales-Forcasting-description
A machine learning model to forecast Walmart weekly sales using historical, economic, and weather data. Feature engineering included time-based, lag, and rolling mean features to improve temporal pattern detection.

📌 The goal is to help improve inventory planning, staffing, and promotional strategies by providing accurate forecasts for future.

📦 Dataset
The dataset is obtained from Kaggle’s Walmart Store Sales Forecasting competition.
It contains 6,435 records from multiple Walmart stores, covering several years of historical weekly sales data.

🎯 Target Variable
Weekly_Sales – a continuous numeric variable representing total sales per store per week.

🛠 Data Preprocessing Steps
Cleaned Column Names – removed extra spaces from headers.

Handled Missing Values – filled using forward/backward fill to preserve time-series continuity.

Feature Engineering – created lag and rolling mean features to capture temporal dependencies.

Date Decomposition – extracted multiple time-based features for seasonal trend learning.

Feature Selection – ensured training and prediction datasets had identical feature sets.

📊 Exploratory Data Analysis (EDA)
Holiday Impact: Notable sales spikes during holidays like Thanksgiving and Christmas.

Store Performance: Significant differences between stores — some consistently outperform others.

Correlation Analysis:

Economic factors (CPI, fuel price, unemployment) have weaker correlations but still add predictive value.

Lag and rolling mean features improve model’s ability to learn trends.

🤖 Model Building & Evaluation
We trained and compared two models:

🚀 Linear regression

🚀 XGBoost Regressor

Advantages: High accuracy with proper tuning, fast inference.

📌 Future Predictions with Dummy Data

To simulate forecasting, we created dummy future inputs for upcoming weeks with expected temperature, fuel price, CPI, and unemployment values.
Lag and rolling features were populated using the most recent historical data, ensuring feature alignment with the training process.
The model then produced Predicted_Weekly_Sales for those future weeks, showing realistic seasonal trends.

🧠 Technologies Used
🐍 Python

📊 Pandas, NumPy – data cleaning & feature engineering

⚙️ Scikit-learn – RandomForestRegressor, preprocessing

🚀 XGBoost – gradient boosting model

📈 Matplotlib, Seaborn – visualizations & trend analysis
