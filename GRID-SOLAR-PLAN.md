# Grid-Level Solar Farm for Denver — Site Plan

## The Pivot

The current site makes a residential rooftop case. Darius wants to make the case for **utility-scale solar farms** on Colorado's Front Range. Same data backbone (NREL, Handmer), completely different argument.

## What Changes

| Residential (current) | Grid-Scale (new) |
|---|---|
| $2.80/W installed | $0.70–1.00/W installed (utility PPA) |
| 10 kW system | 100–500 MW farm |
| Rooftop, south-facing | Ground-mount, single-axis tracking |
| Net metering / bill savings | PPA pricing / wholesale market |
| 25-year homeowner ROI | LCOE vs. gas/coal/wind |
| Individual decision | Policy / investment / municipal case |

## Proposed Structure

### 1. The Cost Collapse (keep & expand)
- The Handmer/IRENA learning curve data still anchors this
- Add utility-scale specific cost curves (NREL ATB data)
- **Key stat:** Utility solar LCOE is now ~$24/MWh unsubsidized — cheaper than operating existing coal plants

### 2. Why the Front Range Specifically
- Same DNI/irradiance advantage (6.12 kWh/m²/day — our existing NREL data)
- **Land availability** — Eastern plains of Colorado: flat, cheap, low-value agricultural land
- **Transmission proximity** — Front Range load centers (Denver, Boulder, Fort Collins, Colorado Springs) are right there
- **Altitude advantage** — same atmospheric clarity argument, but now applied to tracking arrays
- **Grid need** — Colorado's grid is 63% fossil, Xcel has committed to 80% clean by 2030

### 3. The Economics at Scale
- LCOE comparison: solar vs. gas peaker vs. coal vs. wind (Colorado-specific)
- PPA pricing trends in WECC/SPP markets
- Land cost: Eastern CO ag land ~$1,500–3,000/acre vs. solar revenue ~$800–1,200/acre/year
- Job creation: construction + O&M for 200 MW farm
- Tax revenue to rural counties (often the real political unlock)

### 4. Solar + Storage at Grid Scale
- Battery costs at utility scale ($100–150/kWh pack level, falling)
- 4-hour duration batteries making solar dispatchable
- Xcel's own Colorado solar+storage RFP results
- Replace gas peakers entirely — the arbitrage math
- Handmer's transmission vs. batteries argument scales up beautifully here

### 5. Colorado Policy & Regulatory Landscape
- SB21-264: 80% GHG reduction by 2030 for electric sector
- Xcel Energy's Clean Energy Plan
- Colorado PUC IRP proceedings
- Federal IRA incentives (still available for utility-scale, unlike residential)
- Energy community bonus credits for coal transition areas (Pueblo, Craig)

### 6. The Land Use Question
- "But it takes too much land" — debunk with math
- A 500 MW solar farm = ~3,500 acres. Colorado has 24 million acres of cropland.
- Agrivoltaics: sheep grazing under panels, pollinator habitat
- Compare land use to coal mining footprint in NW Colorado

### 7. Denver's Demand Story
- Population growth → load growth
- Data center boom on the Front Range (AI demand)
- EV adoption curve in Colorado (one of the fastest-growing states)
- Electrification of heating (heat pump mandate trajectory)
- All roads point to needing way more clean generation

### 8. Case Studies
- Xcel's Rush Creek wind farm (pivoted to solar comparison)
- NREL's own campus solar
- Pueblo solar farms near the old coal plant
- National examples: Gemini (Nevada), Mammoth (Indiana)

## Data Sources We Already Have
- ✅ NREL Solar Resource API (DNI, GHI for Denver)
- ✅ NREL PVWatts (production modeling)
- ✅ Casey Handmer blog posts (cost curves, batteries, synthetic fuels)
- ✅ EIA Colorado electricity profile
- ✅ EPA eGRID (CO₂ emissions)

## Data Sources We Need
- [ ] NREL Annual Technology Baseline (ATB) — utility solar LCOE projections
- [ ] Lazard LCOE analysis (latest edition)
- [ ] Colorado PUC / Xcel IRP filings — planned solar capacity
- [ ] WECC/SPP wholesale electricity prices
- [ ] Eastern CO land values (USDA)
- [ ] Colorado solar job data (Solar Foundation / IREC)
- [ ] IRA utility-scale incentive details (ITC/PTC current rates)

## Tone & Audience
- **Primary audience:** Local policymakers, municipal leaders, Xcel stakeholders, investors, informed citizens
- **Secondary:** Denver tech community, sustainability-minded homeowners who want the bigger picture
- **Tone:** Data-heavy, Handmer-inspired techno-optimism. Not advocacy fluff — real numbers, real citations. "Here's what the math says, and the math is overwhelming."

## Relationship to Current Site
Two options:
1. **Replace** — pivot the whole site to grid-scale, archive residential as a subpage
2. **Expand** — add grid-scale as a major new section/page, keep residential as the "what you can do" companion

Recommend **Option 2**: the residential case becomes "what this means for your roof" while the main argument is the grid-level transformation. They reinforce each other.

## References from Current Site (Casey Handmer)
- "Solar panels are a revolutionary technology — inert glass rectangles that, placed on the ground, print out wealth at roughly 100x the rate of the best farm land."
  → This quote literally describes a solar farm. Perfect anchor.
- "Batteries and transmission are in direct competition... the outcome is not in doubt."
  → Grid-scale storage argument
- "Storing electricity is hard, but storing heat is easy."
  → Industrial/district heating applications
- Terraform Industries synthetic fuels
  → Grid-scale solar as chemical feedstock. Colorado as a fuel-producing state.
- 48% learning rate, 446 GW deployed in 2024
  → All utility-scale relevant

## Next Steps
1. Darius to confirm structure/approach
2. Research phase: pull NREL ATB, Lazard, Colorado PUC data
3. Build the grid-scale page(s)
4. Update existing site to frame as companion piece
5. Push to GitHub Pages
