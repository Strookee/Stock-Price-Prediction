Stock Price Prediction using CNN + LSTM
📌 Introduction

Stock markets are dynamic, highly volatile, and influenced by numerous economic, social, and political factors. Accurately predicting stock prices is challenging because traditional statistical models often fail to capture the non-linear patterns and sequential dependencies present in financial data.

This project leverages deep learning, specifically a hybrid model combining Convolutional Neural Networks (CNNs) and Long Short-Term Memory networks (LSTMs), to predict stock prices from historical data. The goal is to explore how hybrid models can enhance prediction accuracy compared to using a single approach.

📊 Dataset

The dataset used in this project is provided as Data.csv.

It contains historical stock price information with attributes such as Date, Open, High, Low, Close, and Volume.

For this project, the ‘Close’ price is used as the main feature for prediction.

The dataset is preprocessed into sliding windows so that the model learns both short-term and long-term dependencies in stock price trends.

⚙️ Methodology
1. Data Preprocessing

Handled missing values and formatted the dataset.

Normalized the closing prices for faster and stable training.

Created input sequences (Target-3, Target-2, Target-1) and outputs (Target).

2. Model Architecture

The project uses a hybrid deep learning model:

CNN (Convolutional Neural Network)
Extracts short-term local patterns in stock price movements.

LSTM (Long Short-Term Memory network)
Captures long-term temporal dependencies and sequential patterns in financial time series data.

By combining CNN and LSTM, the model leverages the strengths of both — CNN’s pattern recognition and LSTM’s sequence learning.

3. Training

Split data into training (70%), validation (15%), and testing (15%) sets.

Optimizer: Adam

Loss function: Mean Squared Error (MSE)

Evaluation metric: Root Mean Squared Error (RMSE)

4. Visualization

After training, model predictions were compared with actual stock prices. Graphs were plotted to show how closely the predictions follow the true stock price trends.

📈 Results

The CNN + LSTM hybrid model showed good prediction accuracy compared to standalone models.

It successfully captured both short-term fluctuations and long-term trends in stock prices.

Visualization graphs demonstrated that predicted values follow actual values closely, proving the model’s effectiveness.

🚀 Future Work

Extend the dataset to include macroeconomic indicators (GDP, interest rates, news sentiment).

Try attention mechanisms to improve learning of important time steps.

Deploy the model as a real-time stock price prediction web app.

✅ Conclusion

This project demonstrated how CNN + LSTM hybrid models can be effectively applied to stock price prediction.

CNN extracts short-term local patterns.

LSTM captures long-term sequential dependencies.

Together, they enhance prediction performance compared to single models.

While no model can predict the stock market with complete certainty, this approach highlights the potential of deep learning in financial forecasting and can serve as a stepping stone toward building intelligent decision-support tools for trading and investment.
