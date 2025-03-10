# Stock-Price-Movement_-202401100400181

Overview
This project is designed to fetch, analyse, and visualize short-term stock price movement using historical stock data. It utilizes the yfinance library to retrieve stock prices and employs matplotlib for visualization. Additionally, a simple moving average (SMA) is calculated to help identify stock trends over a short period.

Features:
•	Fetches historical stock data for a given symbol within a specified date range.
•	Plots stock closing prices over time.
•	Computes a 5-day moving average to smooth out short-term fluctuations and highlight trends.
•	Customizable parameters for stock selection and trend analysis.

Usage Instructions
1. Modify Configuration Variables
Edit the following variables in the script to specify the stock symbol and time period:
stock_symbol = "AAPL" # Replace with your desired stock symbol
start_date = "2024-02-01"  # Start date in YYYY-MM-DD format
end_date = "2024-03-01"  # End date in YYYY-MM-DD format
2. Run the Script
Execute the script using Python:
python stock_price_plot.py
3. Interpret the Output
The script will generate two plots:
1.	A Stock Price Movement Chart, which displays the closing prices of the selected stock.
2.	A Trend Analysis Chart, overlaying a 5-day moving average to highlight trends.
   
Customization
•	Change the Stock Symbol: Modify stock_symbol to fetch data for different stocks, e.g., GOOGL, MSFT, TSLA.
•	Adjust the Date Range: Modify start_date and end_date to analyse different timeframes.
•	Modify the Moving Average Window: By default, the script calculates a 5-day moving average. You can adjust this by changing the rolling window:
•	stock_data["MA_X"] = closing_prices.rolling(window=X).mean()
Replace X with the desired number of days.

Example Output
Here are the key insights you can derive from the charts:
•	The general direction of stock price movement (uptrend/downtrend).
•	Identification of short-term fluctuations using the moving average.
•	Possible support and resistance levels based on price trends.

Potential Enhancements
•	Implement additional trend indicators like exponential moving averages (EMA) or Bollinger Bands.
•	Add functionality for user input to select stocks dynamically.
•	Integrate real-time stock data fetching for live analysis.
