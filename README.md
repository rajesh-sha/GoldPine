# GoldPine — Gold Liquidity Sweep PRO v4.4

Institutional **liquidity / price-action** signal indicator for XAUUSD (TradingView Pine v6).

v4.4 keeps every v3.2 label + StochRSI rail — only tidier spacing and clearer pastel colors.

## What desks actually trade (not EMA noise)

**Inducement → External sweep → CISD/MSS → Premium/Discount + OTE → CE/OB/Breaker → opposite pool**

| Edge | Role |
|------|------|
| PDH/PDL, Asia, Day/Week, EQH/EQL, rounds | Liquidity pools |
| Internal → External nesting | Inducement filter |
| MSS / CISD | Structure confirmation after sweep |
| Premium / Discount | Only buy discount, sell premium |
| OTE 62–79% | Optimal Trade Entry of displacement |
| Consequent Encroachment | 50% of FVG/OB entry |
| Breaker at broken swing | Failed structure shelf |
| NY Midnight / Day / Week opens | Institutional magnets |
| SMT Gold vs Silver | True swing divergence (not EMA) |
| Pure Liquidity mode | EMA/Stoch/200MA never veto |

## Files

- `Gold Liquidity Sweep PRO.txt` — paste into TradingView
- `indicators/Gold_Liquidity_Sweep_PRO_v3_Signals.pine` — same script

## Chart setup

1. `OANDA:XAUUSD` on **1 minute**
2. Pine Editor → paste full file → Add to chart
3. Confirm title **v4** and table shows **PURE**
4. Keep Entry Style = `MSS + FVG/OB (PRO)`

## Defaults (v4)

- Pure Liquidity mode: **ON**
- Bias EMA / StochRSI / PTJ 200MA: **OFF as vetoes**
- Prem/Disc, OTE, CE, Breaker, Opens, Nesting, SMT: **ON**

## Disclaimer

Educational only. Not financial advice.
