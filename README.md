# ☀️ The Case for Solar in Denver, CO

A data-driven, single-page website making the case for residential solar power in Denver, Colorado. All solar data comes from real NREL (National Renewable Energy Laboratory) APIs.

## Live Demo

*Not yet deployed — see [DEPLOY.md](DEPLOY.md) for options.*

## Features

- **Real NREL Data** — Solar irradiance from NREL Solar Resource API, production estimates from PVWatts v8
- **City Comparison** — Denver vs Phoenix, LA, Miami, Chicago, Seattle using real DNI data
- **Interactive Calculator** — Slide your monthly bill, get personalized system size, cost, savings, and CO₂ impact
- **Monthly Production Chart** — Actual PVWatts output for a 10kW system with 40° tilt
- **Responsive Design** — Works on mobile, tablet, and desktop
- **No Dependencies** — Single HTML file, vanilla CSS/JS, Google Fonts only external resource
- **Print-Friendly** — Clean output for offline sharing

## Data Sources

| Source | Data Used |
|--------|-----------|
| [NREL Solar Resource API](https://developer.nrel.gov/docs/solar/solar-resource-v1/) | DNI, GHI, and tilt irradiance for 6 cities |
| [NREL PVWatts v8](https://developer.nrel.gov/docs/solar/pvwatts/v8/) | Monthly/annual production for Denver (station 484137) |
| [EnergySage](https://www.energysage.com/local-data/solar-panel-cost/co/denver-county/denver/) | Pricing, payback, savings (March 2026) |
| [EIA](https://www.eia.gov/electricity/state/colorado/) | Colorado electricity rates and grid mix |
| [EPA eGRID](https://www.epa.gov/egrid) | CO₂ emissions factor for Colorado |
| [NOAA/NWS](https://www.weather.gov) | Climate normals (1991-2020) |
| Casey Handmer's research | Solar learning curves, battery economics |

Raw data files are stored in `data/` for reference and reproducibility.

## Project Structure

```
denver-solar/
├── index.html          # The site (single file, ~59KB)
├── index.original.html # Original v1 backup
├── CNAME              # Custom domain config (for Surge.sh)
├── DEPLOY.md          # Deployment instructions
├── README.md          # This file
└── data/
    ├── nrel-solar-resource.json  # Raw NREL irradiance data
    ├── nrel-pvwatts.json         # Raw PVWatts production data
    └── noaa-climate.json         # Denver climate normals
```

## Key Denver Solar Facts (from NREL)

- **DNI**: 6.12 kWh/m²/day (beats Miami at 5.04, LA at 5.72)
- **Annual Production**: 16,524 kWh for a 10kW system
- **Capacity Factor**: 18.9%
- **Best Month**: March (1,536 kWh) — cool temps + rising sun angle
- **Worst Month**: December (1,207 kWh) — still 79% of peak

## Calculator Methodology

The interactive calculator uses these Denver-specific parameters:

- **Rate**: $0.16/kWh (EnergySage, March 2026)
- **Rate increase**: 3% annually
- **Install cost**: $2.80/W (EnergySage market average)
- **Output**: 1,652 kWh/kW/year (NREL PVWatts)
- **Degradation**: 0.5% annually
- **CO₂ factor**: 0.85 tons/MWh (EPA eGRID Colorado)

## Development

No build step required. Just open `index.html` in a browser:

```bash
# Local preview
cd denver-solar
python3 -m http.server 8888
# Open http://localhost:8888
```

## License

Content and code are free to use. Data sourced from public U.S. government APIs (NREL, NOAA, EIA, EPA).

---

*Built March 2026 with real data, not vibes.* 🌞
