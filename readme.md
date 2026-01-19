📈 Stock Price Prediction using Linear Regression
📝 Project Overview
This project focuses on predicting future stock closing prices based on historical market data. Using a synthetic dataset that mimics real-world stock movements (Random Walk), the model utilizes features such as Opening Price, High, Low, and Trading Volume to forecast the next day's Closing Price.

🚀 Key Features
Synthetic Data Generation: Simulated 1,000 days of stock data using numpy and pandas.

Feature Engineering: Implemented data shifting to create a target variable (Next_Close) for supervised learning.

Time-Series Logic: Applied a chronological split (80% Train / 20% Test) instead of a random split to maintain the integrity of time-series data.

Feature Scaling: Used StandardScaler to normalize features, ensuring faster convergence and better accuracy for the regression model.

📊 Technical Workflow
Data Collection: Created a random walk price series with added market noise.

Preprocessing: Handled missing values (from shifts) and standardized numerical inputs.

Model Selection: Employed Linear Regression as a baseline model to understand price trends.

Evaluation: Assessed performance using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R²) score.

📈 Visualizations
The project includes graphical representations to validate the model:

Actual vs. Predicted Plot: A line chart showing how closely the model's predictions follow real market trends.

Residual Analysis: A distribution plot of errors to check for model consistency and bias.

🛠️ Installation
To run this project locally:

Bash

# Clone the repository
git clone https://github.com/YourUsername/Stock-Price-Prediction.git

# Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn
🧪 Results
The model achieves a high R-squared score, indicating a strong correlation between the selected features and the future closing price. The low MAE suggests that the predicted prices are, on average, very close to the actual values.