#Financial Risk Analysis for NVIDIA (NVDA) Stock
____________________________________________________________________________________________________________________________________________________________________________________
Project Description

This project involves a comprehensive analysis of NVIDIA (NVDA) stock data to calculate various risk metrics and visualize the results. The metrics calculated include Value at Risk (VaR), Expected Shortfall (ES), Sharpe Ratio, Sortino Ratio, Maximum Drawdown, and Beta. Additionally, the project involves plotting the distribution of daily returns and a box plot of the calculated risk metrics.
____________________________________________________________________________________________________________________________________________________________________________________
License

BSD 2-Clause License

Copyright (c) 2024, Omkar Sabnis

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
____________________________________________________________________________________________________________________________________________________________________________________
Table of Contents

Installation
Data Source
Risk Metrics
Visualization
Output
____________________________________________________________________________________________________________________________________________________________________________________
Installation

To run this notebook, you'll need to have Python installed along with the necessary libraries. Install the required libraries using the following command:

bash
Copy code
pip install pandas numpy matplotlib seaborn yfinance statsmodels
____________________________________________________________________________________________________________________________________________________________________________________
Data Source

The stock data for NVIDIA (NVDA) is fetched from Yahoo Finance using the yfinance library. The data range is set to the last three years from the current date.
____________________________________________________________________________________________________________________________________________________________________________________
Risk Metrics

The following risk metrics are calculated in this notebook:

Value at Risk (VaR): Measures the potential loss in value of an asset with a given confidence interval over a specified time period.
Expected Shortfall (ES): Also known as Conditional VaR, it represents the average loss given that the loss is beyond the VaR threshold.
Sharpe Ratio: Measures the risk-adjusted return of an asset, considering both positive and negative returns.
Sortino Ratio: Similar to the Sharpe Ratio but only considers downside risk.
Maximum Drawdown: Represents the maximum observed loss from a peak to a trough.
Beta: Measures the volatility of an asset compared to the overall market (S&P 500 in this case).
____________________________________________________________________________________________________________________________________________________________________________________
Visualization

Two main visualizations are provided:

Distribution of Daily Returns: A histogram with a kernel density estimate (KDE) to show the distribution of daily percent changes in the adjusted close price of NVDA.
Box Plot of Risk Metrics: A box plot to visualize the distribution of the calculated risk metrics.
Usage

Open the Notebook: Open financial_data_analysis_for_nvda_stock.ipynb in Jupyter Notebook.
Run the Cells: Execute each cell to fetch NVIDIA stock data, compute risk metrics, and generate visualizations.
Review the Output: Check the results and visualizations in the output cells.
____________________________________________________________________________________________________________________________________________________________________________________
Example Output

Here are some examples of the output generated by this notebook:

VaR: There is a 95 percent chance that NVDA will not lose more than X.XX percent of its value in any given day.
ES: On the worst 5 percent of days, the average loss is Y.YY percent.
Sharpe Ratio: The asset has a risk-adjusted return that is Z.ZZ times the risk-free rate when considering both positive and negative returns.
Sortino Ratio: The asset has a risk-adjusted return that is W.WW times the risk-free rate when considering only negative returns.
Maximum Drawdown: The asset has experienced a maximum loss of V.VV percent from its peak to trough.
Beta: The asset is B.BB times more/less volatile than the stock market.

