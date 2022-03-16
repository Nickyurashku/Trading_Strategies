# Trading Strategies vs Traditional Passive Investing

## Introduction

In this data analysis, I will be testing out 3 different and popular trading strategies versus the traditional buying and holding investment approach. In this analysis, we will see if our strategies can beat the market.

## About the Data

The data is I used in this data analysis the stocks from the DOW Jones Industrial index are pulled from Wikipedia: https://en.wikipedia.org/wiki/Dow_Jones_Industrial_Average. Compiling all the closing prices, we are able to see the trend of the DJI.

![DJI](https://user-images.githubusercontent.com/41551746/158533851-76b3474f-7a79-4ee3-9b28-d22c6bcc340f.png)

## Backtesting a Momentum Strategy vs Buying and Holding the DJI

The first momentum strategy will do the following: if ends in a negative closing price, we will short the market the next day. However, if we end the trading day in the positive, we will go long (hold) the position. This strategy will be tested against just buying the DJI and doing nothing. 

Here are the results of the trade:

![Momentum vs Holding](https://user-images.githubusercontent.com/41551746/158534550-924f6b7c-755a-4f66-9fb0-55d2fe8ae6d6.png)

We observe that trying to time the momentum of the market does not work. In fact we see that our momentum strategy has reduced our portfolio by -4% while the buy and hold strategy provides 11%.

![Screenshot 2022-03-16 000327](https://user-images.githubusercontent.com/41551746/158534721-71043854-2240-489c-b2d7-8d9802705ef8.png)

## Going Against the Momentum

When reveresing our momentum strategy, meaning to short when the market closes in the green the next day to go long when the market is red, we actually see a profit appear of 4%.

![Screenshot 2022-03-16 000718](https://user-images.githubusercontent.com/41551746/158535247-c326d896-0db0-4ec6-af53-9ee386003ed9.png)

However, even though this strategy was profitable, it came no where near our buy and hold strategy.

## Timing the Market with Moving Averages vs. Buying and Holding

The last strategy to test was a popular moving averages strategy. By first smoothing out our average curves by taking 200 day averages and 50 day averages, we used the following technique for trading: when the 50 day moving average crossed above the 200 day moving average we held. However, when the 50 day moving average dropped below 200 day moving average, we shorted the market.

Unfortunately, this strategy was also unsuccessful. Giving us a negative return of -1%.

![Screenshot 2022-03-16 001306](https://user-images.githubusercontent.com/41551746/158536157-a0ef3c48-7a23-4fd0-9afc-e41598efe794.png)

## Conclusion

We tested three different strategies against the traditional buy and hold method. The traditional buy and hold method delievers investors an averge return of 11%. Whereas our active strategies either resulted in negative returns or returns much less than the traditional method. The startegy that was most promising was to trade against the momentum. My belief is that this active trading strategy outperformed others is because it took advantage of price jumps that would trend too high or too low and therefore have a high probablility of regressing back to the mean. Futhermore, we saw that this strategy did in some years outperform the traditional buy and hold method in years 2010 - 2012 and briefly in 2020 during the stock market crash of March. 




