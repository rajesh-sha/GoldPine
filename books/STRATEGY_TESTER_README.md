# Strategy Tester — Gold Liquidity Sweep PRO v6.7.8

## Paste
https://raw.githubusercontent.com/rajesh-sha/GoldPine/cursor/gold-liq-sweep-pro-v3-09e0/GOLD_STRATEGY_PASTE_THIS.txt

## Important (why it looked broken)
v6.7.7 defaults were too strict for backtests (news blackout sits inside NY hours, PRO path rarely completes).  
**v6.7.8** turns **TESTER MODE** on by default and uses fixed size = 1.

## Install fresh (required)
TradingView keeps old settings. Do this:
1. Remove the old strategy from the chart
2. Paste v6.7.8 → Save
3. Add to chart again
4. Title must say **STR v6.7.8**
5. Open Strategy Tester

## Settings to confirm
- Strategy Tester → **TESTER MODE** = ON
- Position sizing = **Fixed size** (1)
- Symbol: TVC:GOLD or OANDA:XAUUSD, 1m

Not financial advice — for study/backtest only.
