<h1>Chukwunonso - Stock Trading Algorithm

<h2>Description</h2>
 This project focuses on the development of an intelligent algorithmic trading system designed to predict and trade Intel Corporation (INTC) stock based on both technical price patterns and real-time market sentiment. The core innovation lies in integrating Natural Language Processing (NLP) with traditional trading algorithms to capture the emotional tone of market news and its influence on short-term price movements.
Using the VADER sentiment analyzer, the system evaluates news headlines and summaries related to Intel Corp, sourced directly from the Finnhub API, which provides up-to-date financial news. Each article is scored for sentiment, and a real-time sentiment bias is computed. This bias acts as a decision filter, modifying the trading algorithm’s behavior—enhancing or suppressing buy/sell signals based on market mood.
The trading logic itself is rooted in a trend-following strategy that detects breakouts, retests, and price rejection patterns. The sentiment bias layer introduces additional context, aiming to avoid entries when sentiment contradicts technical signals and increasing confidence when both align.
I hope you enjoy this one!
<br />

<h2>Languages and Utilities Used</h2>

- <b>Python, Anaconda
- Jupyter Notebook
- VADER SentimentIntensityAnalyzer (NLTK)
- Finnhub API (News endpoint)
- MetaTrader 5 / TradingView (for execution integration)</b>

<h2>Environments Used </h2>

- <b>Windows 11</b> (21H2)

<h2>Project Opener:</h2>
This trading bot focuses on Intel Corporation (INTC) and is built around a price-action strategy enhanced with real-time sentiment analysis. The same logic can be applied to other stocks — you just need to change the ticker symbol and sentiment source. I used one of my earlier trading strategies that detects breakouts, retests, and price rejection patterns, and combined it with VADER sentiment analysis using Intel-related news headlines fetched from the Finnhub API.
The sentiment layer runs separately and scores each news headline as positive, negative, or neutral. Based on the average sentiment of the last 7 days, the bot filters trading signals — avoiding trades during negative sentiment and boosting confidence when sentiment aligns with technical signals. This gives the algorithm more context beyond just price movement.
Like my forex bot, this version also stores the logic in functions like df = detect_support_resistance(df, window=10), df = detect_breakout_retest(df), and df = detect_trade_signals(df). The visualizations you’ll see are outputs from the strategy, though the full algorithm code is not shared for privacy. Thank you!
<br />

<h2>Fetching Intel Stock Data:</h2>
<img src="https://imgur.com/sCbF8G3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Downloading VADER lEXICON:</h2>
<img src="https://imgur.com/LEaHxLI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Testing VADER samples for scoring and bias:</h2>
<img src="https://imgur.com/ZCRQyHn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Load the AG News dataset from Hugging Face and Retrieving over 1300 INTEL related news from AG News:</h2>
<img src="https://imgur.com/rzcselB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/042lPMi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Creating and averaging sentiment scores from AG for trading bias:</h2>
<img src="https://imgur.com/ugOqmGP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Loading last 7 days of FINNHUB News and Retrieving over 70 INTEL related news:</h2>
<img src="https://imgur.com/GLFD3BD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Creating and averaging sentiment scores from FINNHUB for trading bias:</h2>
<img src="https://imgur.com/cc7X8eh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Trading Algorithm:</h2>
<h2>Transforming and cleaning data:</h2>
<img src="https://imgur.com/fBpB8cc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Detecting Trends, highs and lows:</h2>
<img src="https://imgur.com/g918QaZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Detecting Support and Resistance levels:</h2>
<img src="https://imgur.com/j5eaCoT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Detecting Breakouts and Retests to give trade signals:</h2>
<img src="https://imgur.com/DxpgMTu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Adding Stoploss and Takeprofits to each trade:</h2>
<img src="https://imgur.com/p0SMPRS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Visualization of Algorithm Winrate over the last 48 hours of trading INTC WITHOUT sentiment included:</h2>
<img src="https://imgur.com/U9ZP5EC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Active trading bot printing trading status:</h2>
<img src="https://imgur.com/jSxc52H.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



















<h2>Applying Risk Management to trades:</h2>


<h2>Testing my Trading Bot:</h2>
I had to put the bot in a while loop to continuously scan the market every 5 minutes for trading opportunities, I changed this later on to scan every 10 seconds to prevent missing trading opportunities and keep my results consistent.
<img src="https://imgur.com/axdqg6g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<h2>Successful Trade executions and exits status:</h2>


<h2>Some Trade results:</h2>







# Forex-Trading-Robot
Forex Trading Algorithm #AlgorithmicTrading #TradingRobot #DataAutomation
