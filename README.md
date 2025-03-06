# Data-Science-Intern-Assignment
# Algorithmic Trading Project

## Overview

This project focuses on analyzing financial data, developing predictive models, and implementing an algorithmic trading strategy. It includes data preprocessing, feature engineering, machine learning-based price prediction, backtesting a trading strategy with stop-loss and take-profit mechanisms, and optimizing model performance.

## Tasks Completed (As Per Assignment PDF)

### **Task 1: Data Analysis and Feature Engineering**

- **Data Collection**: Loaded historical stock price data (`ALB.csv`).
- **Preprocessing**: Handled missing values, removed NaNs, and computed stock returns.
- **Feature Engineering**: Created key technical indicators:
  - **Simple Moving Averages (SMA_10, SMA_50)**
  - **Relative Strength Index (RSI)**
  - **Moving Average Convergence Divergence (MACD)**
  - **Volatility**
  - **Momentum**
- **Visualization**: Plotted stock prices and technical indicators to identify trends.

### **Task 2: Model Building**

- **Data Preparation**:
  - Defined **features (`X`)** and **target (`y`)** for price movement prediction.
  - Split data into **training (80%)** and **testing (20%)**.
- **Model Training**:
  - Implemented a **Random Forest Classifier** to predict whether the stock price will go up or down.
- **Model Evaluation**:
  - Measured accuracy, precision, recall, and F1-score.
  - Generated a confusion matrix for performance assessment.

### **Task 3: Backtesting a Trading Strategy**

- **Implemented a Simple Trading Strategy**:
  - **Buy** if the model predicts price increase.
  - **Sell** if the model predicts price decrease.
- **Risk Management**:
  - Added **Stop-Loss (2%)** to limit losses.
  - Added **Take-Profit (4%)** to secure gains.
- **Simulated Trading Execution**:
  - Ran backtesting over historical data.
  - Compared strategy returns to a buy-and-hold approach.

### **Task 4: Optimization and Refinement**

- **Hyperparameter Optimization**:
  - Used **GridSearchCV** to fine-tune the Random Forest model.
  - Optimized parameters such as `n_estimators` and `max_depth`.
- **Strategy Refinement**:
  - Evaluated the impact of additional technical indicators.
  - Improved model performance for better trading decisions.

## Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Backtrader (for optional strategy testing)

## Files

- `Untitled1.ipynb`: Jupyter Notebook containing the full implementation.
- `ALB.csv`: Historical stock data used for analysis.

## How to Run

1. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn backtrader
   ```
2. Open `Untitled1.ipynb` in Jupyter Notebook.
3. Run all cells sequentially to execute the entire workflow.
4. Analyze outputs including model performance, visualizations, and backtesting results.

## Results

- Predictive model accuracy and performance metrics.
- Stock trend visualizations with technical indicators.
- Final capital after applying the backtested trading strategy.

## Conclusion

This project successfully demonstrates the use of **machine learning for stock price prediction** and **algorithmic trading**. By engineering relevant financial indicators and training a **Random Forest model**, we were able to classify price movements effectively. The **backtesting strategy** provided insights into **trading performance and risk management techniques**. The combination of predictive modeling and **trading strategy execution** showcases the potential of **data-driven decision-making in financial markets**.

