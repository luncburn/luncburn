# WELCOME TO LUNC BURN PREDICTION PAGE

The purpose of this page is to share the collected data on the LUNC coin, with an aim to provide the data necessary to answer one and only question :"When is LUNC going to reach $1.0 USD per 1 LUNC coin?"

We will start collecting the data, daily, and then, we will add several prediction algorigthms such as time series prediction, etc.

Currently, we are collecting the data from Coin Marketcap.

header.csv is the header file

data.csv is the collected data


Each day, we are making one call and updating the data.csv table


The header.csv contains:
total_supply - the toal supply that has been minted (not to be confused with a circulating supply)

circulating_supply - The amount of circulating LUNC coins

cmc_rank - How does LUNC compare to other coins on the rank list?

last_updated - when was the information in data.csv file updated?

last_updated_ts - timestamp presentation of last updated for the purpose of doing the time series

price - current LUNC price

volume_24h - How much money has been transferred in the past 24hr

volume_change_24h,percent_change_1h,percent_change_24h,percent_change_7d,percent_change_30d,percent_change_60d,percent_change_90d,market_cap,market_cap_dominance,fully_diluted_market_cap,last_updated_p,last_updated_p_ts,calculated_burn_days
