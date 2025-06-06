# CoinML - Cryptocurrency Machine Learning Dataset

## Overview
A comprehensive collection of cryptocurrency historical data for machine learning analysis. This dataset includes price, volume, and market data for major cryptocurrencies, perfect for time series analysis, price prediction models, and market research.

## Features
- **Multi-Cryptocurrency Data**: 23 major cryptocurrencies included
- **Historical Time Series**: Comprehensive historical price data
- **Machine Learning Ready**: Pre-formatted CSV files for easy analysis
- **Market Coverage**: Popular coins including Bitcoin, Ethereum, and altcoins
- **Research Grade**: Clean, structured data suitable for academic and commercial research

## Cryptocurrencies Included
- **Bitcoin (BTC)** - The original cryptocurrency
- **Ethereum (ETH)** - Smart contract platform
- **Cardano (ADA)** - Proof-of-stake blockchain
- **Polkadot (DOT)** - Multi-chain protocol
- **Chainlink (LINK)** - Decentralized oracle network
- **Litecoin (LTC)** - Peer-to-peer cryptocurrency
- **Monero (XMR)** - Privacy-focused cryptocurrency
- **Dogecoin (DOGE)** - Meme-based cryptocurrency
- **Binance Coin (BNB)** - Exchange token
- **Solana (SOL)** - High-performance blockchain
- **XRP** - Digital payment protocol
- **Stellar (XLM)** - Cross-border payment network
- **Tether (USDT)** - Stablecoin
- **USD Coin (USDC)** - USD-backed stablecoin
- **Aave (AAVE)** - DeFi lending protocol
- **Uniswap (UNI)** - Decentralized exchange token
- **Cosmos (ATOM)** - Interoperable blockchain
- **EOS** - Blockchain platform
- **IOTA (MIOTA)** - IoT-focused cryptocurrency
- **Tron (TRX)** - Entertainment blockchain
- **NEM (XEM)** - Enterprise blockchain
- **Crypto.com Coin (CRO)** - Exchange and payment token
- **Wrapped Bitcoin (WBTC)** - Tokenized Bitcoin

## Data Structure
Each CSV file contains cryptocurrency market data with columns typically including:
- Date/Timestamp
- Open Price
- High Price
- Low Price
- Close Price
- Volume
- Market Cap (where available)

## Technologies Used
- **CSV Format** - Universal data format
- **Time Series Data** - Historical market information
- **Python Compatible** - Ready for pandas, numpy analysis
- **R Compatible** - Ready for R statistical analysis

## Getting Started

### Prerequisites
- Python 3.x with pandas, numpy
- R with data.table (optional)
- Jupyter Notebook (recommended)
- Machine learning libraries (scikit-learn, TensorFlow, PyTorch)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/oskarcode/coinml.git
   cd coinml
   ```

2. Load data in Python:
   ```python
   import pandas as pd
   
   # Load Bitcoin data
   bitcoin_data = pd.read_csv('coin_Bitcoin.csv')
   ethereum_data = pd.read_csv('coin_Ethereum.csv')
   ```

3. Load data in R:
   ```r
   library(data.table)
   
   # Load Bitcoin data
   bitcoin_data <- fread('coin_Bitcoin.csv')
   ethereum_data <- fread('coin_Ethereum.csv')
   ```

## Usage Examples

### Price Prediction Model
```python
import pandas as pd
from sklearn.ensemble import RandomForestRegressor

# Load data
df = pd.read_csv('coin_Bitcoin.csv')

# Prepare features for ML model
# ... feature engineering code ...

# Train model
model = RandomForestRegressor()
model.fit(X_train, y_train)
```

### Market Analysis
```python
import matplotlib.pyplot as plt

# Load multiple cryptocurrencies
coins = ['Bitcoin', 'Ethereum', 'Cardano']
data = {}

for coin in coins:
    data[coin] = pd.read_csv(f'coin_{coin}.csv')

# Comparative analysis
# ... analysis code ...
```

## Applications
- **Price Prediction Models**: LSTM, ARIMA, Prophet forecasting
- **Market Analysis**: Correlation studies, volatility analysis
- **Portfolio Optimization**: Risk assessment and allocation
- **Trading Algorithms**: Backtesting and strategy development
- **Academic Research**: Cryptocurrency market behavior studies
- **Risk Management**: Value at Risk (VaR) calculations

## Data Quality
- Data sourced from reliable cryptocurrency exchanges
- Cleaned and validated for consistency
- Missing values handled appropriately
- Suitable for production ML models

## Contributing
Contributions are welcome! Please feel free to:
1. Fork the project
2. Add new cryptocurrency data
3. Improve data quality
4. Submit pull requests

## License
This project is open source and available under the [MIT License](LICENSE).

## Disclaimer
This data is for educational and research purposes only. Not financial advice. Always do your own research before making investment decisions.

## Contact
- GitHub: [@oskarcode](https://github.com/oskarcode)
- Project Link: [https://github.com/oskarcode/coinml](https://github.com/oskarcode/coinml)

## Acknowledgments
- Cryptocurrency exchanges for providing market data
- The crypto community for supporting open data initiatives

---
*Cryptocurrency data for machine learning and market analysis*