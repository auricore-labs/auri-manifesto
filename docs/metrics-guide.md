# 📊 Auri Metrics Guide

## Core metrics
- **Lead Time:** Doing → Done. Target ≤ 2 days/card.  
- **Throughput:** delivered cards per flow. Target ≥ 80% planned.  
- **Bug Density:** bugs/deliveries. Target ≤ 0.2.  
- **Cycle Health:** `(1 - BugDensity) × (OnTime/Total)`. Target ≥ 0.85.  
- **Technical Debt:** weighted sum (1–5). Target ≤ 10.

## Weekly ritual (15 min, async‑first)
1. Review Lead Time trend.  
2. Check Throughput vs planned.  
3. Count Bugs and Debt.  
4. If Cycle Health < 0.8 → switch next flow to stabilization.  

## Forecasting
```
forecast_days = lead_time_avg * planned_cards
```

## Dashboard tips
- GitHub Projects / Linear auto‑capture start/finish times.  
- Show 3 bars: Lead Time, Throughput, Bugs.  
