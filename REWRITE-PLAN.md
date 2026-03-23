# Denver Solar Site Rewrite Plan

## Goal
Rewrite the site to be more like Casey Handmer's blog: analytical, data-driven, written for an informed audience. Less startup landing page, more scientific essay with good data visualization.

## Content Direction

### Tone
- Direct, analytical prose. No marketing copy ("Solar City", "What Are You Waiting For?")
- Assume the reader is smart. Don't explain what solar panels are.
- Lead with data and physics. Use specific numbers.
- Acknowledge tradeoffs honestly (payback period is 13 years — say so plainly)
- Handmer-style: conversational but rigorous

### Section Restructure

1. **Header/Intro** — Simple. "Solar Economics in Denver, CO." Brief thesis: Denver's physical geography and current energy costs make rooftop solar a strong economic proposition. No hero animations or badges.

2. **The Physics: Why Denver** (replaces "Denver's Natural Advantage")
   - Elevation → reduced atmospheric scattering → higher DNI. Quantify it.
   - Semi-arid climate → fewer cloudy days. Temperature coefficient: cold panels are efficient panels.
   - Compare DNI to other cities with actual NREL data (keep this — it's good data)
   - Drop the emoji cards. Use prose with inline data.

3. **Solar vs. Gas: What Electricity Actually Costs** (replaces "Solar Costs Have Collapsed")
   - Colorado's grid is ~40% natural gas, ~18% coal
   - Natural gas LCOE: $39-101/MWh (Lazard), but retail to consumers: $160/MWh
   - Rooftop solar LCOE in Denver: ~$72/MWh with zero fuel cost and falling
   - Utility-scale solar: $24-96/MWh — already cheaper than new gas
   - Key insight: solar has zero marginal cost and zero fuel price risk. Gas does not.
   - Include the learning curve data but as context, not the whole section

4. **Real Production Data** (keep, clean up)
   - NREL PVWatts monthly output — this is strong data, keep it
   - Simplify presentation

5. **Solar + Batteries: The Utilization Tradeoff** (replaces "The Battery Revolution")
   - Incorporate Handmer's model: for loads <$1000/kW, intermittent solar wins; above that, batteries
   - A typical home (~$2000/kW appliance capex) is firmly in battery-backed territory
   - Denver capacity factor (0.19) means ~4.5 peak sun hours/day
   - Battery sizing: 13.5 kWh covers ~5 hours at average draw
   - Cost: batteries at $45/kWh cell level, ~$200-300/kWh installed (Powerwall ~$700/kWh retail, but falling)
   - Xcel Battery Connect rebate ($350/kW up to $5K)

6. **The Winter Question** (keep but tighten)
   - Shorter. One paragraph + the data. December DNI > Chicago's annual average. Done.

7. **Economics** (replaces "The Numbers" and "Calculator")
   - System cost, payback, 25-year savings — keep the calculator but embed it cleanly
   - Colorado incentives as a subsection, not its own giant section
   - Be honest: 13-year payback without federal ITC is long. But: zero fuel cost, rising grid rates, home value increase.

8. **Conclusion** — Brief. Replace the CTA sales pitch. "The data supports it. Here's where to get quotes."

### Remove
- "The Bigger Picture" section (synthetic fuels, datacenters — tangential)
- Sales-y CTA section
- Leaderboard link (keep the page but don't make it a nav item)
- Hero animations, badge, stat counter animations

## Styling Direction

### Design
- **White background, black text** — clean, bright, minimal
- Serif or clean sans-serif body font (system fonts are fine)
- Charts/data viz: simple bars with muted colors on white
- No dark mode, no gradients, no glowing effects
- Generous whitespace
- Think: academic paper meets good blog post
- Cards → paragraphs with data inline. Fewer boxes, more prose.

### Specific CSS Changes
- Background: white (#fff or #fafafa)
- Text: near-black (#111 or #1a1a1a)  
- Accent: a single muted color for charts (blue or amber)
- Font: system stack or Inter at normal weights
- Max-width: ~720px (reading width)
- No fixed nav — simple top header
- No animations or hover effects
- Tables: clean, minimal borders
- Charts: simple horizontal bars, thin, labeled clearly

## Files to Modify
1. **index.html** — Full rewrite (content + styling)
2. **leaderboard.html** — Restyle to match (white/minimal)
3. **tracker.html** — Restyle to match (white/minimal)

## Reference Files
- `ref/handmer-solar-batteries.md` — Handmer article summary
- `ref/research-data.md` — EIA, Lazard, NREL data for cost comparisons
- Current `index.html` — existing structure/data to preserve what's good
