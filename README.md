# samplebotcode

Language: Python 

Kucoin Trading Bot:

This code provides the (crude) outline for a more complex and customizable cryptocurrency trading bot currently in use. This bot is initiated through the direct user input of a future date into the variable labeled 'futuree' in mainbot and running the code.

The bot takes positions in asset increments of {1.00, 1.01, 1.02...} multipled by the normalization units (here .18) - i.e. the first position of any asset will be worth the equivalent of .18 USDT or .000065 BTC, the second .1818, and so on. Cover positions are initiated when the price of the asset falls more than .5% away from the initial target price. For this version of the bot, there are seven such cover positions at various levels of price changes away from the initial target.

The full version of this bot is customizable - the parameters for <1) the magnitude and frequency of cover positions 2) asset balances 3) normalization units 4) percent changes that initialize positions 5) list of assets> are all user-defined and set according to user-defined end targets for 1) account balances 2) length of time. As an example of one customization feature, the normalization unit may be set and iteratively increased according to a moving average of successful positions.

The code is almost entirely my original work. I have written it with minimal references, save the 1) Kucoin API documentation and 2) todays_date_function. I have deliberately refrained from providing detailed annotations. 
