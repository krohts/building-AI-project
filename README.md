# AI empowered crypto currency trading system

Final project for the Building AI course

## Summary

This project is about merging the two hottest topics of today – crypto currencies (aka bitcoin, ethereum and altcoins) and AI – into a relatively simple AI empowered crypto currency trading system.


## Background

More and more retail traders are driven to make a fortune in crypto currency trading. Unfortunately, human psychology is far too often on the way. Feelings of arousal and stress tend to impair one’s trading performance. Fear of losing, fear of missing out, fear of letting a profit turn into a loss and fear of not being right tend to cause human traders ‘getting screwed’ by the market even if they had all the knowledge. In addition, manually searching for trading opportunities is cumbersome and once one gets tired, one starts making mistakes. Last but not least, in case of human traders there is always a lot of difficult-to-track subjectivity involved.

Scanning through the vast amounts of data and performing rational calculations (trading is a probability game, after all!) is where the machines excel. On the other hand, humans have the ability to see the broader context, incl. factors that are not included in the models, and put things into perspective. 

These are my considerations when coming to the space of cryptocurrency trading. I believe that AI can come handy in tasks like identifying market trends and expecting ‘pumps and dump’ of certain assets. This is especially true on the cryptocurrency market as the space is still not crowded by the institutional traders.

The ultimate goal of the project is to join the strengths of humans and machines to leverage the strengths and compensate for the weaknesses of both. AI is ought to give ‘buy’ and ‘sell’ signals with proper location of stop-loss and limit orders as applicable; the machine should also output its ‘reasoning’ for each signal. It is then about human to decide whether to execute on the signal or not. (In order to continue improving the algorithm, the final decision and accompanying human judgement should be recorded as well.)

To start with, there scope is limited in several respects when it comes to trading strategies, incl.:
* No leverage
* No short selling
* No derivatives, no exotic instruments
* Only basic types of orders assumed (market order, limit order, stop order).
In other words, there is going to be nothing overly complex or risky from the trading realm which a retail trader should better not use.


## How is it used?

First, I intend to develop the solution for my own trading. Going forward, many retail traders might benefit from the project in the same way as I do – assuming that the project successfully executed and properly escalated.

A conceptual model of my envisioned AI-based trading solution is depicted on the figure below. Of course, there are other considerations out of the scope of current project that enter into the ‘calculation’, incl. risk management principles, transaction costs and taking portfolio-wide view. For now, these other considerations would be based on human judgement.

[Pic to be added!]


## Data sources and AI methods

First, I intend to develop the solution for my own trading. Going forward, many retail traders might benefit from the project in the same way as I do – assuming that the project successfully executed and properly escalated.

Daily trading stats on cryptos can be downloaded from https://coinmarketcap.com. Further data points to be ‘scraped’ include but are not limited to:
* Crypto Fear & Greed Index (e.g.: https://alternative.me/crypto/fear-and-greed-index/)
* Popularity of the search word ‘bitcoin’ (e.g.: Google Trends)
* S&P 500 index data (e.g.: Yahoo! Finance)
* U.S. Dollar Index (e.g.: MarketWatch)
* isc. data points from TradingView

Considering feasibility aspect, the AI techniques involved would be as simple as possible but not simpler. The current idea is to apply logistic regression as the AI issues in project scope are classification issues based on the numerical data. At the same time, there are many opportunities to expand in future: using deep learning for chart pattern recognition and text mining when it comes to sentiment analysis based on news headings, social media comments – just to name a few.

All the programming will be done in Python and, if necessary, in other open-source languages such as R.


## Challenges

Currently I see the following main risks to the project:
<ol>
<li> Getting stuck in details </li>
<li> The scope of the project expanding beyond what is feasible, given the available resources </li>
<li> There is no guarantee that a working solution will be found </li>
</ol> 

The way to address the first two challenges is to focus on delivering minimum viable product (MVP). Further refinements and upgrades are always possible in later iterations. As for the third challenge, even if no working solution is found this time, gained knowledge about what does NOT work is also valuable.

Other challenges include my fairly limited practical experience with trading and with crypto. Furthermore, coding skills and machine learning skills need to be constantly improved. These are the kind of challenges that motivate me; I am eager to learn.

Assuming successful implementation, there are still going to be several limitations:
* Most definitely, project outcome is not going to be a ‘money-making-bot’ one might dream of. (I think that chances of inventing a true ‘money-making-bot’ are about the same as the chances of coming up with a perpetual motion machine. ALL algorithms need to be properly maintained and updated as necessary.) 
* There will not be any API connections with any specific trading platform; all trades would have to be finally decided by a human and executed manually.
* The algorithm will cover only the basics of what a professional trader typically does and considers (think of most basic order types, most basic technical indicators, limited timeframes etc.).
* No solution is developed for tracking the actual trades in real-time for later backtesting purposes.


## What next?

Next steps in the project execution are as follows:
* Business understanding (trading; crypto currencies) & defining the MVP in detail
* Data gathering / writing data gathering scripts
* Writing data preparation scripts, incl. programmatically defining technical indicators, trendlines, S/R levels, chart patterns etc. looked for by the traders (here, there are bits and pieces of open-source code available – it is about finding out and connecting the dots)
* Programmatically defining the model output variable(s)
* Model development, experimenting with various options
* Developing an AI based trading strategy, incl. backtesting the strategy on the data available till date
* Writing clean scripts for implementation

The above steps only provide a rough guidance. Inherently, modelling process is not something straightforward. Instead, the process is iterative and often returns back to the previous step. 

When it comes to further product development, the basic conceptual model developed in frame of the current project (see section ‘How is it used’) can be incorporated into a full-fledged algorithmic trading strategy as illustrated below. 

[Pic to be added!]

Once there is a working solution (product), there would be several options for building a business model around it. One example would be simply selling there trading signals to professional quant hedge funds. Legally more complicated yet more noble model would be contributing to the success of retail traders (e.g.: introducing a subscription-based service).


## Acknowledgments

* Hacker Noon author Rafael Schultze-Kraft for demonstrating how simply ‘throwing’ complex algorithms to the price data does NOT work and for sharing his Python code for inspiration: https://hackernoon.com/dont-be-fooled-deceptive-cryptocurrency-price-predictions-using-deep-learning-bf27e4837151 
