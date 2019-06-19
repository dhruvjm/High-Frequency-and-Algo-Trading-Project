# High-Frequency-and-Algo-Trading-Project

Assignment #3

Goal:
The purpose of this assignment is to find out if and when an order should be immediately executed by paying (half) the Bid/Offer spread or if would be economically better to rest this order withing the Bid/Offer spread for a period time to achive possibly a better execution.

Data:
You have received for a given instrument (Gbp/Usd) a large set of tick data (for both Bid and Offer). Note that no information about offered sizes was given to you.
In addition a set of orders covering the same time period was also given to you.

Method(s):
You will explore and quantify two approaches
1)	Market Taking (MT) -- for each order, you will agress the market immediately and therefore incurr the (half) Bid/Offer spread
2)	Opportunistic Market Making (OMM) -- for each order, you will rest it within the Bid/Offer spread for a given amount of time awaiting for its (possible) opportunistic execution
a.	I suggest that you carry this second approach in two ways:
i.	First by joining “your side” of the market (ie the Bid price if you are buying, the Offer if selling) -- OMMSide
ii.	Secondly by resting your order at mid market -- OMMMid
b.	In both cases, you will define (and choose a value) for a max Stop Loss (SL) in case the market runs away from you. If it is the case, you will then aggress the market to fill your order
c.	Again in both cases, you will also define (and choose a value) for a max Time to Execution (TTE). Upon reaching this time limit, you will aggress the market to fill your order
3)	Note that you will always assume that there is enough liquidity to 100% fill you upon the execution of your order
4)	Furthermore assume also that upon execution of your order you are done at your expected price (no slippage upon your order’s execution) 




Analysis:
1)	For each of your 3 approaches (MT, OMMSide and OMMMid), provide a recapitulating table which will show at the minimum the average and median execution PnL for each order (taken from Mid Market), average and median time to execution), the number of times when your Stop Loss was triggered, the number of times when your order was executed on Time Limit.

2)	Add other statistics if you wish (for extra points)
3)	List in annex each trade with its PnL, time to execution and whether its SL or TTE has been triggered.


Further Analysis:
1)	Show the influence of the length of TTE on the median execution PnL – present a graph

2)	Each order was labelled as either DIS or MAR or SOM. These are three different alpha generators. Can you find any significant differences in term of execution


