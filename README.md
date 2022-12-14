# WELCOME TO LUNC BURN PREDICTION PAGE

The purpose of this page is to share the collected data on the LUNC coin, to provide the data necessary to answer only one question: "When is LUNC going to reach $1.0 per 1 LUNC coin?"

We will start collecting the data, daily, and then, we will add several prediction algorithms such as time series prediction, etc.

Currently, we are collecting the data from Coin Marketcap.

header.csv is the header file, tab delimited

data.csv is the collected data, tab delimited




The header.csv contains:

total_supply - the total supply that has been minted (not to be confused with a circulating supply) [LUNC]

circulating_supply - The amount of circulating LUNC coins [LUNC]

cmc_rank - How does LUNC compare to other coins on the rank list? [Number]

last_updated - when was the information in data.csv file updated? [Date]

last_updated_ts - timestamp presentation of last updated to do the time series [Number]

price - current LUNC price [USD]

volume_24h - How much money has been transferred in the past 24hr [USD]

volume_change_24h - The change in 24h volume [USD]

percent_change_1h - self-explanatory [Percent USD]

percent_change_24h - self-explanatory [Percent USD]

percent_change_7d - self-explanatory [Percent USD]

percent_change_30d - self-explanatory [Percent USD]

percent_change_60d - self-explanatory [Percent USD]

percent_change_90d - self-explanatory [Percent USD]

market_cap - self-explanatory [LUNC]

market_cap_dominance - self-explanatory 

fully_diluted_market_cap - self-explanatory

last_updated_p - when was percentage data last updated [Date]

last_updated_p_ts - last update as linux timestamp [Number]

calculated_burn_days - how many days it will take to burn LUNC [Days]


## Note on calculated_burn_days

First, the circulating supply in LUNC and the market cap in USD must be equal for the price to be $1

Therefore, we calculate this difference as the number of tokens to be burned

Then, we apply the price to the number of tokens to see that is their USD value

We apply 1.2% to daily volume, and then simply derive how many days it would take to burn all USD.


In other words, the formula is:
((circulating_supply - market_cap) * price) / (volume_24h * 0.012)

### Why is calculated_burn_days calculation wrong?
It is wrong simply because we are assuming that circulating_supply, market_cap, volume_24h and price are constants.  This is by no means true, and therefore, we can apply the power of AI to help us predict the actual number of days.  However, we need to collect the data first. Once enough data is collected, this page will be updated with the predictions, prediction graphs, method explanations etc. calculated_burn_days is just an intermediate step.

