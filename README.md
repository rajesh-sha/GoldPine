# GoldPine — Gold Liquidity Sweep PRO v5

Institutional **liquidity / price-action** signal indicator for XAUUSD (TradingView Pine v6).

v5 keeps the v3.2 visual language (pastel labels, StochRSI rails, light table) and adds a desk-grade **Elite Edge Pack**.

## Sequence desks trade

**HTF Draw → Inducement → External sweep → CISD/MSS → Prem/Disc + OTE → CE/OB/Breaker/IFVG/Unicorn → opposite pool / draw target**

| Edge | Role |
|------|------|
| PDH/PDL, Asia, Day/Week, EQH/EQL, rounds | Liquidity pools |
| HTF Draw on Liquidity | Only buy toward BSL / sell toward SSL |
| HTF POI (1H FVG) | LTF entry aligned with higher-TF shelf |
| Power of 3 (AMD) | Asia ACC → London MAN → NY DIST |
| Internal → External nesting | Inducement filter |
| MSS / CISD | Structure confirmation after sweep |
| Premium / Discount + OTE + CE | Entry quality |
| IFVG / Unicorn / BPR | Failed FVG, breaker+FVG, balanced range |
| NDOG / NWOG | Day/week opening gaps |
| SMT Gold vs Silver + DXY | True swing divergence |
| News blackout + A+ mode | Stand aside / strict confluence |

## Files

- `Gold Liquidity Sweep PRO.txt` — paste into TradingView
- `indicators/Gold_Liquidity_Sweep_PRO_v3_Signals.pine` — same script

## Chart setup

1. `OANDA:XAUUSD` on **1 minute**
2. Pine Editor → paste full file → Add to chart
3. Confirm title **v5.0**
4. Keep Entry Style = `MSS + FVG/OB (PRO)`
5. Optional: turn **A+ ONLY mode** ON for fewer, higher-quality signals

## Defaults (v5)

- Pure Liquidity mode: **ON**
- HTF Draw required: **ON**
- AMD / POI / IFVG / Unicorn / NDOG / BPR / Time / News: **ON**
- A+ ONLY mode: **OFF** (turn on when you want strict desk filter)
- Bias EMA / StochRSI / PTJ 200MA: **OFF as vetoes**

## Disclaimer

Educational only. Not financial advice.
