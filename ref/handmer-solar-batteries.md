# Casey Handmer: Solar and Batteries for Generic Use Cases
# Source: https://caseyhandmer.wordpress.com/2024/11/09/solar-and-batteries-for-generic-use-cases/

## Key Points

### Solar Economics
- Solar PV learning rate: 44% cost reduction per doubling of cumulative deployment, ~15% cheaper per year
- 2024: 446 GW deployed globally (= entire global nuclear fleet, ~1 MW/min)
- China alone: 160 GW in 9 months
- Cheapest panels: $0.07/W (below trend)
- "Inert glass rectangles that, placed on the ground, print out wealth at roughly 100x the rate of the best farm land"

### Battery Economics
- Battery learning rate: 23% cost reduction per doubling of cumulative deployment
- Recent lows: $45/kWh (cell level) — previously unthinkable

### Solar+Battery Utilization Model
- Used real NREL solar performance data (5-min increments, full year)
- Assumptions: $200k/MW solar PV, $200k/MWh battery storage

#### Key Finding: Two Stable Strategies
1. **Low capex loads (<$1000/kW):** Intermittent operation with modest solar oversizing. No batteries needed. Utilization ~0.21–0.33
2. **High capex loads (>$1000/kW):** Battery-backed daily charge/discharge. Sharp transition.

#### Detailed Results:
- $10/kW load: Solar array = load size, utilization 0.21
- $1000/kW load: 2.4x solar overbuild, utilization 0.33 (pure solar peak shaving)
- $10,000/kW load: 8.3x solar overbuild, 15 kWh/kW battery, utilization 0.94
- Beyond 15 kWh/kW battery: diminishing returns. Better to overbuild solar.
- AI datacenter ($50,000/kW): ~0.98 utilization is cost-optimal (~170 hrs/yr downtime)

#### Power Cost
- Solar + battery amortized over 10 years: $12–$50/MWh over most utilization range
- "Far lower than any other electricity source"
- Even 99.9% uptime only requires extra solar build
- Below 0.3 utilization: pure solar, no batteries
- 0.3–0.9: solar + battery (equal cost at ~0.5)
- Above 0.9: mostly solar overbuild (cheaper than rarely-used batteries)

### Style Notes (for content rewrite)
- Direct, analytical prose
- No marketing language
- Leads with data and physics
- Uses specific numbers throughout
- Charts tell the story; text provides context
- Assumes an informed reader
- Acknowledges tradeoffs honestly
