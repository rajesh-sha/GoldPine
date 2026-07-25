# GoldPine — Gold Liquidity Sweep PRO v6.1

Institutional **liquidity / price-action** signal indicator for XAUUSD (TradingView Pine v6).

**v6.1 = complete daily playbook** (all 10 checklist edges).

## Sequence

**Daily bias lock → Judas / SB path → Sweep → CISD/MSS → Disp+FVG → Prem/Disc + OTE → CE/OB → Asia or -0.27 TP1 → PDH/PDL/draw TP2**

| # | Edge | Status |
|---|------|--------|
| 1 | Daily bias narrative (lock BUY/SELL before London) | Done |
| 2 | True Judas (Asia against bias → disp+FVG → MSS with bias) | Done |
| 3 | Displacement + FVG gate | Done |
| 4 | Silver Bullet model (swing sweep → MSS → FVG) | Done |
| 5 | TP1 Asia opposite / -0.27 expansion | Done |
| 6 | IPDA 20/40/60 day magnets | Done |
| 7 | London close / NY lunch dead hours | Done |
| 8 | SMT Gold vs Ag + DXY + **ES** | Done |
| 9 | One trade per killzone | Done |
| 10 | News windows (CPI/NFP/FOMC manual) | Done |

## Files

- `Gold Liquidity Sweep PRO.txt` — paste into TradingView
- `indicators/Gold_Liquidity_Sweep_PRO_v3_Signals.pine` — same script

## Chart setup

1. `OANDA:XAUUSD` on **1 minute**
2. Paste full file → Add to chart
3. Confirm title **v6.1**
4. Entry Style = `MSS + FVG/OB (PRO)`
5. Tune **Daily Playbook (v6.1)** + news windows to your CPI/NFP/FOMC times

## Disclaimer

Educational only. Not financial advice.
