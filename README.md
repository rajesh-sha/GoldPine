# GoldPine — Gold Liquidity Sweep PRO v6.0

Institutional **liquidity / price-action** signal indicator for XAUUSD (TradingView Pine v6).

v6 keeps the v3.2 look + v5 elite edges, and adds a plain-English **Daily Playbook** for intraday Gold.

## Sequence desks trade

**HTF Draw → Inducement → External sweep → CISD/MSS → Prem/Disc + OTE → CE/OB/Breaker/IFVG/Unicorn → opposite pool / draw target**

| Edge | Role |
|------|------|
| PDH/PDL, Asia, Day/Week, EQH/EQL, rounds | Liquidity pools |
| Daily Bias (midnight/day open + 4H) | Preferred side before London |
| Judas fake-move window | London open trap path (fake one side → reverse) |
| Strong displacement gate | Hard push required after the fake |
| Silver Bullet hour + 1 trade/KZ | Clean delivery hour / anti-overtrade |
| TP1 = Asia opposite | Classic Judas first target |
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
3. Confirm title **v6.0**
4. Keep Entry Style = `MSS + FVG/OB (PRO)`
5. Settings group **Daily Playbook (v6)** — Daily Bias / Judas / Displacement / Silver Bullet

## Defaults (v6)

- Pure Liquidity mode: **ON**
- Daily Bias guide: **ON** (require = OFF)
- Judas window: **ON** (require path = OFF)
- Strong displacement: **ON**
- Silver Bullet boost: **ON** (SB-only = OFF)
- TP1 Asia opposite: **ON**
- Max 1 signal per killzone block: **ON**
- HTF Draw required: **ON**
- A+ ONLY mode: **OFF**

## Disclaimer

Educational only. Not financial advice.
