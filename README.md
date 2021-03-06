# 0xbtc-discord-price-bot
bot to monitor/post price etc to the 0xbtc discord server

Installation:
 - copy `template_secret_info.py` to `secret_info.py` and fill in your bot's authentication settings
 - Install python 3
 - `pip3 install websocket discord`
 - `python3 main.py`

Requires:
 - python3
 - websocket
 - discord

Todo:
 - allow price command to show price of objects ie `!price lambo`
 - typos/new commands
   - !pools
   - !marketcap
 - multiple quick commands will run in parallel, causing some things like 
   command counter to only count 1/2 commands. Results should really be pushed
   to a queue instead.
 - catch `discord.errors.Forbidden` when commands are run in forbidden channels
 - Need a new 'Pairing' class to handle pairings in a more generic way. This
   will allow easier integration of BTC pairings (ie mercatox)
 - volume_eth and volume_usd are not strictly defined - sometimes it means total
   volume across all pairs (converted to eth), sometimes it means volume in eth
   only and volume_btc means volume in btc only.
 - ATH announcements
 - 24h high/low/average
 - ascii chart?
 - new exchanges
   - tokenjar [link](https://tokenjar.io/0xbtc)
   - tokenstore [link](https://token.store/trade/0xBTC)
   - payfair [link](https://payfair.io/?coin=0XBTC&tradeType=sell&currency=USD)
   - instex [link](https://app.instex.io/0xBTC-WETH)
   - cryptobridge (not yet)
 - ~~combine prices from multiple sources~~
 - ~~0xBTC - BTC ratio~~
 - ~~!likenewfordtaurus~~
 - ~~!usedtaurus~~
 - ~~!avocadoontoast avocadotoast~~
 - ~~! price all~~
 - ~~!vol~~
 - ~~!zj~~