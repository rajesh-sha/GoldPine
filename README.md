# GoldPine — Gold Liquidity Sweep PRO v3

Institutional liquidity-sweep signal indicator for **XAUUSD** (TradingView Pine Script v6).

Not a retail “buy the wick” tool. It encodes the sequence desks actually trade:

**Pool → Sweep → CISD/MSS → Order Block / FVG retest → opposite liquidity**

## Files

| File | Purpose |
|------|---------|
| `Gold Liquidity Sweep PRO.txt` | Main indicator (paste into TradingView Pine Editor) |
| `indicators/Gold_Liquidity_Sweep_PRO_v3_Signals.pine` | Same script, `.pine` extension |

## Chart setup

1. Symbol: `OANDA:XAUUSD` (tick volume) or your gold feed
2. Timeframe: **1 minute**
3. Pine Editor → paste script → Add to chart
4. Create alerts from the script’s alertconditions / `alert()` messages

## What v3 adds (vs v2)

| Edge | Why it matters |
|------|----------------|
| **MSS / CHoCH confirmation** | A sweep alone is suspicion; body-close through the swing that ran into the pool is confirmation |
| **CISD arm** | Early opposite-delivery close after the sweep |
| **Order Block + FVG entry** | Enter on institutional displacement zone retest, not the sweep candle |
| **Round-number pools** | Gold stop shelves at $10 handles |
| **Session hierarchy** | London vs Asia (Judas), NY vs London — confluence bonus |
| **Sweep quality / double-sweep SL** | Rejection wick filter + worst-extreme stop while confirming |
| **Stricter default grade** | Default minimum grade **A + B** |

## Default entry mode

**`MSS + FVG/OB (PRO)`** — keep this for maximum edge.

Legacy modes still available:
- `FVG retest`
- `Reclaim close` (more signals, lower quality)

## Status table (how to read it)

- **DO NOT TRADE** — stay-away engine (Friday close-out, news chaos, Bias vs DXY conflict, daily cap, dead market)
- **Institutional setup** — pending sweep → waiting MSS → zone live
- **Session hunt** — Judas / NY-vs-London hierarchy
- **Next action** — plain-English instruction for the current bar

## Recommended filters (pro profile)

- Bias Mode: EMA Filter (4H)
- DXY inverse: ON
- StochRSI exhaustion: ON
- PTJ 200-day MA: ON
- Kill zones only: ON
- Minimum grade: **A + B**
- Entry style: **MSS + FVG/OB (PRO)**

## Disclaimer

Educational tool only. Not financial advice. Past patterns do not guarantee future results. Size risk carefully.
