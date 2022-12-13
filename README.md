# Seasonality of Futures Contracts
This notebook will calculate the seasonality, using seasonal_decompose from the statsmodels library, of the given set of futures contracts by taking a 52-Week Fourier Transform over each contract. 
Using this seasonal frequency, it will buy/long and/or sell/short at respective seasonal lows and highs. 
Plotly was used to display the charts, and allow them to be interactive for better analysis.
I faced problems trying to display the charts in GitHub, so I hope to implement a new version
in the future that is able to display them as static images. For now, I have printed the charts to .png
and attached them to a .pdf for sample viewing. However, if you open this in Colab you will find the charts appear
at the bottom, so please make sure to re-run the notebook and check them out there for more recent data.

# How to use this Project
1. Adjust the portfolio holdings to whatever contracts you would like to determine the seasonality of.
This data is pulled from Yahoo Finance using the yfinance library, so make sure to use the appropriate ticker strings.
2. Adjust the period and interval to your choosing. The default is set to weekly and the seasonal period is 52.
This should give you a yearly seasonal which would be most popular, but if you would like to adjust it you can on line 16 of the Main.
3. Run the main and watch as the charts are created and returns calculated.

# Thank you
Thank you for checking out my notebook, and I hope you find some use for my design.
