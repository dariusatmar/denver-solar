# Research Data for Denver Solar Site Rewrite

## Colorado Electricity Profile (EIA 2024)
- **Primary energy source:** Natural gas
- **Net generation:** 58,798,395 MWh
- **Average retail price:** 12.07 ¢/kWh (state avg), ~16 ¢/kWh (Denver residential)
- **CO₂ emissions:** 25,602 thousand metric tons; 958 lbs/MWh (ranked 16th highest)

## Utility Operating Expenses (EIA 2024, mills/kWh)
- **Fossil Steam Total:** 41.32 mills/kWh ($41.32/MWh) — operation 6.98, maintenance 5.81, fuel 28.52
- **Gas Turbine/Small Scale Total:** 22.95 mills/kWh ($22.95/MWh) — operation 2.25, maintenance 2.11, fuel 18.59
- **Nuclear Total:** 23.08 mills/kWh ($23.08/MWh)

## LCOE Estimates (Lazard LCOE+ 2025, unsubsidized)
- **Utility-scale solar:** $24–96/MWh (midpoint ~$49/MWh)
- **Onshore wind:** $24–75/MWh
- **Natural gas combined cycle:** $39–101/MWh
- **Natural gas peaker:** $115–221/MWh
- **Coal:** $65–152/MWh
- **Nuclear (new build):** $136–189/MWh

## Denver Residential Solar LCOE (calculated)
- Installed cost: $2.80/W → $2,800/kW
- Output: 1,652 kWh/kW/year (NREL PVWatts, Denver)
- 25-year lifetime with 0.5%/yr degradation: ~38,800 kWh lifetime per kW
- **Residential rooftop LCOE: ~$72/MWh ($0.072/kWh), no subsidies**
- Compare: Denver grid rate is $160/MWh ($0.16/kWh) — solar produces at less than half
- Note: Utility-scale solar is even cheaper (~$30–50/MWh in good sites)

## Colorado Generation Mix (approximate)
- Natural gas: ~40%
- Coal: ~18%  
- Wind: ~25%
- Solar: ~8%
- Hydro: ~4%
- Other: ~5%

## Key Comparison: Solar vs. Natural Gas in Denver
| Metric | Rooftop Solar | Grid (Gas-dominated) |
|--------|--------------|---------------------|
| LCOE | $72/MWh | $160/MWh (retail) |
| Fuel cost risk | Zero | Volatile (gas prices) |
| CO₂ | 0 | 958 lbs/MWh |
| Price trend | Falling ~15%/yr | Rising ~3%/yr |
| Lifespan | 25-35 years | Ongoing fuel purchases |

## Handmer's Key Insight for Denver
- Denver solar resource: ~0.19 capacity factor (18.9% from PVWatts)
- This is higher than the Wyoming site Handmer used (~0.17)
- For residential use ($1,000–$2,000/kW appliances): modest overbuild + battery is optimal
- A home battery (13.5 kWh Powerwall) provides ~5 hours backup at average 2.7 kW draw
- Solar+battery amortized: $12–50/MWh over 10 years (Handmer's model)
