# rolling-beta-analysis
# Rolling Beta Analysis and Stability Assessment

## Overview
This project provides a Jupyter notebook for fetching stock price data, calculating rolling betas over different time windows (1Y, 2Y, 5Y), analyzing beta stability, and visualizing the results using Plotly. It focuses on Indian stocks listed on NSE, using the CNX 500 index (^CRSLDX) as the market proxy. The analysis helps in understanding how stock betas evolve over time and their stability.

Key features:
- Fetches historical stock data using yfinance.
- Computes daily returns and rolling betas via linear regression.
- Generates interactive plots for beta evolution and a heatmap for stability metrics (e.g., mean, std, CV of betas).
- Stocks analyzed: BBOX.NS, BEL.NS, VBL.NS, SHANTIGEAR.NS, HDFCBANK.NS, VSTIND.NS.

## Requirements
- Python 3.8+
- Libraries: 
  - yfinance
  - pandas
  - numpy
  - plotly
  - scipy
  - IPython (for display)

Install dependencies:
pip install yfinance pandas numpy plotly scipy ipython


## Usage
1. Clone the repository:
git clone https://github.com/yourusername/rolling-beta-analysis.git
cd rolling-beta-analysis


2. Open the Jupyter notebook:
jupyter notebook Beta_analysis.ipynb


3. Run the cells sequentially:
- Cells 1-6: Import libraries, fetch data, calculate returns and rolling betas.
- Cell 7: Plot beta evolution (saves images/HTML).
- Cell 8: Analyze and print beta stability metrics.
- Cell 9: Create stability heatmap (saves images/HTML).

Outputs include printed statistics, Plotly figures, and saved files like `beta_evolution_timeline.png` and `Beta_stability_heatmap.png`.

## Data Sources
- Stock data from Yahoo Finance (yfinance).
- Period: Last 6 years (adjustable in code).

## Limitations
- Requires internet access for data fetching.
- Beta calculations skip windows with insufficient data.
- Visualizations are optimized for dark theme.

## License
MIT License. Feel free to use and modify.
