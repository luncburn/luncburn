# WELCOME TO LUNC BURN PREDICTION PAGE


The purpose of this page is to share the collected data on the LUNC coin, to provide the data necessary to answer only one question: "''When is LUNC going to reach $1.0 per 1 LUNC coin?''"


Currently, we are collecting the data from Coin Marketcap, and it will take several months after the burn algorithm is implemented to do some valid predictions. The data.csv is updated only once per day.


'''header.csv''' is the header file


'''data.csv''' is the collected data




Each day, we are making one call and update the data.csv table




The header.csv contains:

total_supply - the total supply that has been minted (not to be confused with a circulating supply)


<span style="background-color:#cccccc;">circulating_supply</span> - The amount of circulating LUNC coins


<span style="background-color:#cccccc;">cmc_rank </span>- How does LUNC compare to other coins on the rank list?


<span style="background-color:#cccccc;">last_updated</span> - when was the information in data.csv file updated?


<span style="background-color:#cccccc;">last_updated_ts</span> - timestamp presentation of last updated to do the time series


<span style="background-color:#cccccc;">price</span> - current LUNC price


<span style="background-color:#cccccc;">volume_24h</span> - How much money has been transferred in the past 24hr


<span style="background-color:#cccccc;">volume_change_24h</span> - The change in 24h volume


<span style="background-color:#cccccc;">percent_change_1h</span> - self-explanatory


<span style="background-color:#cccccc;">percent_change_24h</span> - self-explanatory


<span style="background-color:#cccccc;">percent_change_7d</span> - self-explanatory


<span style="background-color:#cccccc;">percent_change_30d</span> - self-explanatory


<span style="background-color:#cccccc;">percent_change_60d</span> - self-explanatory


<span style="background-color:#cccccc;">percent_change_90d</span> - self-explanatory


<span style="background-color:#cccccc;">market_cap</span> - self-explanatory


<span style="background-color:#cccccc;">market_cap_dominance</span> - self-explanatory


<span style="background-color:#cccccc;">fully_diluted_market_cap</span> - self-explanatory


<span style="background-color:#cccccc;">last_updated_p</span> - when was percentage data last updated


<span style="background-color:#cccccc;">last_updated_p_ts</span> - last update as linux timestamp


<span style="background-color:#cccccc;">calculated_burn_days</span> - how many days it will take to burn LUNC



## Note on calculated_burn_days


First, the circulating supply in LUNC and the market cap in USD must be equal for the price to be $1


Therefore, we calculate this difference as the number of tokens to be burned


Then, we apply the price to the number of tokens to see that is their USD value


We apply 1.2% to daily volume, and then simply derive how many days it would take to burn all USD.




In other words, the formula is:

'''((circulating_supply - market_cap) * price) / (volume_24h * 0.012)'''


### Why is this wrong?

It is wrong simply because '''we are assuming that''' '''circulating_supply, market_cap, volume_24h''' '''and''' '''price are constants'''. This is by no means true, and therefore, we can apply the power of AI to help us predict the actual number of days. However, we need to collect the data first. Once enough data is collected, this page will be updated with the predictions, prediction graphs, method explanations etc.


