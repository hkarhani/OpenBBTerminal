```
usage: borrow [-l LIMIT] [--current] [-h] [--export {csv,json,xlsx}]
```

Display DeFi borrow rates. [Source: https://defirate.com/]

```
optional arguments:
  -l LIMIT, --limit LIMIT
                        Number of records to display (default: 10)
  --current             Show Current Borrow Rates or Last 30 Days Average (default: True)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example:
```
2022 Feb 15, 06:05 (✨) /crypto/defi/ $ borrow
                                                                                                             DeFi Borrow Rates
┌────────┬─────────────┬──────────────────────────────────┬──────────────────────────────────┬──────────────────────────────────┬───────────────────────────────────┬──────────────────────────────────┬───────────────────────────────────┐
│ Symbol │ Compound v2 │                       Aave       │                       dYdX       │                       Fulcrum    │                       BlockFi     │                       Nexo       │                       Celsius     │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ DAI    │ 4.09%       │ 3.5%                             │ 0%                               │ 19%                              │ –                                 │ -2%                              │ 1%                                │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ USDC   │ 3.16%       │ 2.96%                            │ 0.01%                            │ 19%                              │ –                                 │ -2%                              │ 1%                                │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ ETH    │ 2.77%       │ 0.12%                            │ 0%                               │ 6%                               │ –                                 │ -2%                              │ 1%                                │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ BTC    │ –           │ –                                │ –                                │ –                                │ –                                 │ -2%                              │ 1%                                │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ WBTC   │ 2.32%       │ 0.32%                            │ –                                │ 3%                               │ –                                 │ –                                │ 1%                                │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ USDT   │ 3.57%       │ 3.04%                            │ –                                │ 19%                              │ –                                 │ -2%                              │ 1%                                │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ MKR    │ 2.33%       │ 0.13%                            │ –                                │ 10%                              │ –                                 │ –                                │ –                                 │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ ZRX    │ 5.74%       │ 0.28%                            │ –                                │ 8%                               │ –                                 │ –                                │ 1%                                │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ REP    │ 3.42%       │ 0.16%                            │ –                                │ 8%                               │ –                                 │ –                                │ –                                 │
├────────┼─────────────┼──────────────────────────────────┼──────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ BAT    │ 3.84%       │ 0.98%                            │ –                                │ –                                │ –                                 │ –                                │ 1%                                │
└────────┴─────────────┴──────────────────────────────────┴──────────────────────────────────┴──────────────────────────────────┴───────────────────────────────────┴──────────────────────────────────┴───────────────────────────────────┘
```