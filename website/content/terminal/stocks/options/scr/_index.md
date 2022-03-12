```
usage: scr [-p {TSLA_Calls_90Days,Highest_OI,template,TSLA_Poots,SPY_ATM_Poots,Long_FAANGM,high_IV,3DTE_Degenerate,SPY_ATM_Calls,Highest_IV,Highest_Volume}] [-l LIMIT] [-h] [--export {csv,json,xlsx}]
```

Screener filter output from https://ops.syncretism.io/index.html. Where: CS: Contract Symbol; S: Symbol, T: Option Type; Str: Strike; Exp v: Expiration; IV: Implied Volatility; LP: Last Price; B: Bid; A: Ask; V: Volume; OI: Open Interest; Y: Yield; MY: Monthly Yield;
SMP: Regular Market Price; SMDL: Regular Market Day Low; SMDH: Regular Market Day High; LU: Last Trade Date; LC: Last Crawl; ITM: In The Money; PC: Price Change; PB: Price-to-book.

```
optional arguments:
  -p {TSLA_Calls_90Days,Highest_OI,template,TSLA_Poots,SPY_ATM_Poots,Long_FAANGM,high_IV,3DTE_Degenerate,SPY_ATM_Calls,Highest_IV,Highest_Volume}, --preset {TSLA_Calls_90Days,Highest_OI,template,TSLA_Poots,SPY_ATM_Poots,Long_FAANGM,high_IV,3DTE_Degenerate,SPY_ATM_Calls,Highest_IV,Highest_Volume}
                        Filter presets (default: high_IV)
  -l LIMIT, --limit LIMIT
                        Limit of random entries to display. Default shows all (default: 10)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example:
```
2022 Feb 16, 09:50 (✨) /stocks/options/screen/ $ scr
                                                                Screener Output
┏━━━━━━━━━━━━━━━━━━━━━┳━━━━━━┳━━━┳━━━━━━━┳━━━━━━━━━━┳━━━━━━┳━━━━━━┳━━━━━━┳━━━━━━┳━━━━━━┳━━━━━━┳━━━━━━┳━━━━━━┳━━━━━━━┳━━━━━━━┳━━━━━━━┳━━━━━━━━━━┓
┃ CS                  ┃ S    ┃ T ┃ Str   ┃ Exp ∨    ┃ IV   ┃ LP   ┃ B    ┃ A    ┃ V    ┃ OI   ┃ Y    ┃ MY   ┃ SMP   ┃ SMDL  ┃ SMDH  ┃ LU       ┃
┡━━━━━━━━━━━━━━━━━━━━━╇━━━━━━╇━━━╇━━━━━━━╇━━━━━━━━━━╇━━━━━━╇━━━━━━╇━━━━━━╇━━━━━━╇━━━━━━╇━━━━━━╇━━━━━━╇━━━━━━╇━━━━━━━╇━━━━━━━╇━━━━━━━╇━━━━━━━━━━┩
│ VIAC220218C00036000 │ VIAC │ C │ 36.00 │ 02-18-22 │ 1.00 │ 1.28 │ 1.28 │ 1.31 │ 4623 │ 3404 │ 0.04 │ 0.68 │ 35.99 │ 34.75 │ 36.03 │ 02-15-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ VXX220225P00020500  │ VXX  │ P │ 20.50 │ 02-25-22 │ 1.00 │ 0.97 │ 0.96 │ 1.00 │ 1552 │ 1525 │ 0.05 │ 0.17 │ 21.39 │ 21.33 │ 22.22 │ 02-15-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ MARA220225C00037000 │ MARA │ C │ 37.00 │ 02-25-22 │ 1.00 │ 0.16 │ 0.16 │ 0.17 │ 118  │ 261  │ 0.00 │ 0.02 │ 28.54 │ 27.44 │ 28.93 │ 02-15-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ RIOT220225C00025000 │ RIOT │ C │ 25.00 │ 02-25-22 │ 1.00 │ 0.16 │ 0.14 │ 0.15 │ 189  │ 1707 │ 0.01 │ 0.02 │ 19.66 │ 18.85 │ 19.76 │ 02-15-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ VIAC220218C00037000 │ VIAC │ C │ 37.00 │ 02-18-22 │ 1.00 │ 0.85 │ 0.86 │ 0.88 │ 2707 │ 2750 │ 0.02 │ 0.44 │ 35.99 │ 34.75 │ 36.03 │ 02-15-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ SKLZ220218C00004500 │ SKLZ │ C │ 4.50  │ 02-18-22 │ 1.00 │ 0.17 │ 0.16 │ 0.17 │ 1828 │ 2241 │ 0.04 │ 0.69 │ 4.46  │ 4.11  │ 4.46  │ 02-15-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ PLUG220218P00023000 │ PLUG │ P │ 23.00 │ 02-18-22 │ 0.99 │ 0.51 │ 0.50 │ 0.52 │ 2078 │ 778  │ 0.02 │ 0.41 │ 23.77 │ 22.08 │ 23.92 │ 02-15-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ BBBY220218C00018500 │ BBBY │ C │ 18.50 │ 02-18-22 │ 0.99 │ 0.15 │ 0.13 │ 0.17 │ 589  │ 905  │ 0.01 │ 0.15 │ 16.66 │ 15.71 │ 16.75 │ 02-15-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ TDOC220218C00091000 │ TDOC │ C │ 91.00 │ 02-18-22 │ 0.99 │ 0.08 │ 0.03 │ 0.05 │ 101  │ 104  │ 0.00 │ 0.01 │ 74.93 │ 72.09 │ 75.14 │ 02-14-22 │
├─────────────────────┼──────┼───┼───────┼──────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┼───────┼───────┼──────────┤
│ PTON220225P00027000 │ PTON │ P │ 27.00 │ 02-25-22 │ 0.99 │ 0.24 │ 0.22 │ 0.25 │ 1040 │ 430  │ 0.01 │ 0.03 │ 33.25 │ 31.96 │ 33.65 │ 02-15-22 │
└─────────────────────┴──────┴───┴───────┴──────────┴──────┴──────┴──────┴──────┴──────┴──────┴──────┴──────┴───────┴───────┴───────┴──────────┘
```