# Markowitz Portfolio Optimization Project with Google Collab

This project is a Google Colab notebook that performs a comprehensive portfolio analysis and optimization using historical market data and AMUNDI & MSCI performance benchmarks. It calculates returns, risk metrics, visualizes performance, and identifies optimal portfolios (Minimum Variance and Maximum Sharpe Ratio) via Monte Carlo simulations.

## 📁 Repository Structure


├── Portfolio Project.ipynb       # Main Colab notebook

├── AMUNDI ACTIONS EURO Performances 2024.xlsx  # Excel file with AMUNDI & MSCI data

└── README.md                    # Project overview and instructions

## 🛠️ Requirements

* Python 3.7+
* Google Colab environment (or local Jupyter notebook)

### Python Libraries

* pandas
* pandas\_datareader
* statsmodels
* numpy
* matplotlib
* seaborn
* scipy
* yfinance
* python-dateutil

You can install the required libraries via:


pip install pandas pandas_datareader statsmodels numpy matplotlib seaborn scipy yfinance python-dateutil

## 🚀 Usage

1. **Clone the repository** to your local machine or open directly in Google Colab:

git clone [https://github.com/](https://github.com/)<your-username>/portfolio-optimization.git
cd portfolio-optimization

   Or, in Google Colab: **File > Open notebook > GitHub >** paste repository URL.

2. **Upload the Excel file**  
   In the first code cell, you’ll be prompted to upload the AMUNDI & MSCI data file:  
   `AMUNDI ACTIONS EURO Performances 2024.xlsx`  
   Make sure the filename matches exactly.

3. **Run all cells** to:
   - Download historical price data for selected tickers (ASML, SAP, NVO, LVMUY, ^STOXX50E, TTE.PA, ^FCHI, SNY, GC=F, CC=F) from Yahoo Finance (2014-02-03 to 2024-01-29).
   - Normalize series to a Base-100 index.
   - Compute daily and yearly log returns.
   - Calculate average return, standard deviation, covariance, and correlation.
   - Perform Monte Carlo simulations (100,000 portfolios) to find the efficient frontier.
   - Identify the Minimum Variance Portfolio and the Maximum Sharpe Ratio Portfolio.
   - Visualize weight distributions and the Efficient Frontier with the Capital Market Line.

4. **Inspect results**:
   - Tables displaying returns, risk metrics, and optimized weights.
   - Plots for performance comparison, weight allocations, and Efficient Frontier.

## ⚙️ Customization

- **Tickers & Date Range**: Edit the `tickers`, `start_date`, and `end_date` variables in the notebook.
- **Portfolio Weights**: Use custom weight vectors or the equally weighted portfolio by modifying the `ptf_weights` or `ptf_equaly_weighted` arrays.
- **Number of Simulations**: Adjust `nb_simulations` for finer optimization at the cost of computation time.

## 🤝 Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
*Happy investing and data analysis!*
