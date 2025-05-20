# Download stock data (e.g., Apple)
ticker = 'AAPL'
data = yf.download(ticker, start='2015-01-01', end='2023-12-31')

# Use only 'Close' prices
df = data[['Close']]
df.dropna(inplace=True)
