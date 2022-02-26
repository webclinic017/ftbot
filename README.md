# ftbot
freqtrade bot configuration for binance spot, with default strategy using WMA (Weighted Moving Average) crossed.

## Pre-requisite
- [Docker](https://docs.docker.com/get-docker/)

## Backtesting on selected pairs from 2021-2022 in 4h timeframe, initial capital 3000 USDT
### BACKTESTING REPORT - Result for strategy WmaCrossed

|       Pair |   Buys |   Avg Profit % |   Cum Profit % |   Tot Profit USDT |   Tot Profit % |     Avg Duration |   Win  Draw  Loss  Win% |
|------------|--------|----------------|----------------|-------------------|----------------|------------------|-------------------------|
|   DOT/USDT |     13 |           8.06 |         104.79 |           936.903 |          31.23 |  2 days, 6:09:00 |    10     3     0   100 |
|   KMD/USDT |     12 |           7.88 |          94.57 |           928.778 |          30.96 |  1 day, 10:40:00 |     9     3     0   100 |
| AUDIO/USDT |     15 |           5.64 |          84.59 |           683.721 |          22.79 |  2 days, 5:52:00 |     7     8     0   100 |
|  CELR/USDT |     22 |           4.83 |         106.34 |           644.571 |          21.49 |  3 days, 7:05:00 |    15     6     1  68.2 |
|   LTC/USDT |     17 |           4.35 |          73.90 |           615.457 |          20.52 | 3 days, 14:49:00 |    12     5     0   100 |
|   ADA/USDT |     22 |           3.73 |          81.99 |           530.827 |          17.69 |  2 days, 7:38:00 |    14     8     0   100 |
|   SOL/USDT |     15 |           3.98 |          59.73 |           530.233 |          17.67 | 2 days, 23:44:00 |     7     8     0   100 |
|   FTM/USDT |     24 |           2.87 |          68.98 |           434.887 |          14.50 | 2 days, 12:40:00 |    15     7     2  62.5 |
|  LINK/USDT |     23 |           2.49 |          57.38 |           425.639 |          14.19 |  3 days, 7:50:00 |    13    10     0   100 |
|   UTK/USDT |     15 |           2.21 |          33.09 |           424.295 |          14.14 | 2 days, 11:44:00 |    10     4     1  66.7 |
|   ETC/USDT |     12 |           3.28 |          39.40 |           371.200 |          12.37 |  2 days, 5:20:00 |     8     4     0   100 |
|   ICP/USDT |      3 |          11.48 |          34.45 |           349.982 |          11.67 |   1 day, 4:00:00 |     2     1     0   100 |
|   QNT/USDT |      1 |          27.87 |          27.87 |           342.934 |          11.43 |         16:00:00 |     1     0     0   100 |
|  QTUM/USDT |     22 |           1.90 |          41.76 |           332.497 |          11.08 | 5 days, 12:55:00 |     8    14     0   100 |
|   YFI/USDT |      8 |           2.78 |          22.26 |           225.126 |           7.50 |  1 day, 15:30:00 |     7     0     1  87.5 |
|      TOTAL |    224 |           4.16 |         931.10 |          7777.049 |         259.23 | 2 days, 21:42:00 |   138    81     5  61.6 |
### BUY TAG STATS
|   TAG |   Buys |   Avg Profit % |   Cum Profit % |   Tot Profit USDT |   Tot Profit % |     Avg Duration |   Win  Draw  Loss  Win% |
|-------|--------|----------------|----------------|-------------------|----------------|------------------|-------------------------|
| TOTAL |    224 |           4.16 |         931.10 |          7777.049 |         259.23 | 2 days, 21:42:00 |   138    81     5  61.6 |

### SELL REASON STATS
|   Sell Reason |   Sells |   Win  Draws  Loss  Win% |   Avg Profit % |   Cum Profit % |   Tot Profit USDT |   Tot Profit % |
|---------------|---------|--------------------------|----------------|----------------|-------------------|----------------|
|           roi |     217 |    136    81     0   100 |           4.96 |        1077.24 |           9233.17 |         153.89 |
|     stop_loss |       5 |      0     0     5     0 |         -29.94 |        -149.7  |          -1494    |         -21.39 |
|   sell_signal |       2 |      2     0     0   100 |           1.78 |           3.56 |             37.87 |           0.51 |
### LEFT OPEN TRADES REPORT
|   Pair |   Buys |   Avg Profit % |   Cum Profit % |   Tot Profit USDT |   Tot Profit % |   Avg Duration |   Win  Draw  Loss  Win% |
|--------|--------|----------------|----------------|-------------------|----------------|----------------|-------------------------|
|  TOTAL |      0 |           0.00 |           0.00 |             0.000 |           0.00 |           0:00 |     0     0     0     0 |

### SUMMARY METRICS
| Metric                 | Value               |
|------------------------|---------------------|
| Backtesting from       | 2020-03-02 00:00:00 |
| Backtesting to         | 2022-02-25 08:00:00 |
| Max open trades        | 7                   |
|                        |                     |
| Total/Daily Avg Trades | 224 / 0.31          |
| Starting balance       | 3000 USDT           |
| Final balance          | 10777.049 USDT      |
| Absolute profit        | 7777.049 USDT       |
| Total profit %         | 259.23%             |
| Trades per day         | 0.31                |
| Avg. daily profit %    | 0.36%               |
| Avg. stake amount      | 805.106 USDT        |
| Total trade volume     | 180343.676 USDT     |
|                        |                     |
| Best Pair              | CELR/USDT 106.34%   |
| Worst Pair             | YFI/USDT 22.26%     |
| Best trade             | DOT/USDT 27.87%     |
| Worst trade            | UTK/USDT -29.94%    |
| Best day               | 448.207 USDT        |
| Worst day              | -489.904 USDT       |
| Days win/draw/lose     | 105 / 564 / 4       |
| Avg. Duration Winners  | 1 day, 8:26:00      |
| Avg. Duration Loser    | 7 days, 0:00:00     |
| Rejected Buy signals   | 69                  |
| Entry/Exit Timeouts    | 0 / 0               |
|                        |                     |
| Min balance            | 3015.12 USDT        |
| Max balance            | 10777.049 USDT      |
| Drawdown (Account)     | 8.25%               |
| Drawdown               | 489.904 USDT        |
| Drawdown high          | 2940.487 USDT       |
| Drawdown low           | 2450.583 USDT       |
| Drawdown Start         | 2021-02-21 00:00:00 |
| Drawdown End           | 2021-02-22 12:00:00 |
| Market change          | 1936.07%            |


## How to Use
### Step 1: [Required]
Configure key & secret, for more info check [this](https://www.binance.com/en/support/faq/360002502072/)
```json

      "exchange": {
        "name": "binance",
        "key": "",
        "secret": "",

```

### Step 2: [Optional]
Setup telegram token & chat_id, if you want to monitor and access the bot via telegram, use this.
```json

    "telegram": {
        "enabled": false,
        "token": "",
        "chat_id": ""
    },
```

### Step 3: [Optional]
Download Data for backtesting,
```bash
docker-compose run --rm freqtrade download-data --config user_data/config.json --exchange binance --days 730 -t 4h
docker-compose run --rm freqtrade backtesting --config user_data/config.json --strategy WmaCrossed --timeframe 20210225-20220225 -i 4h
```



### Step 4: [Optional]
Configure hyperopt
```bash
docker-compose run --rm freqtrade hyperopt --hyperopt-loss SharpeHyperOptLossDaily --spaces roi stoploss trailing --strategy WmaCrossed --config user_data/config.json -e 200
```

### Step 5:
Start the bot
```bash
docker-compose up -d
```

# Note:
- Set the `"dry_run": false` in config.json before running it to live.
- If you have any questions, submit an issue


