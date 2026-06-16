---
name: retrofit-advisor
description: Generate AI-ranked retrofit and decarbonization recommendations with ROI, payback period, energy savings, and carbon reduction for each measure. Use when asked about building retrofits, capex planning, energy upgrades, decarbonization investments, equipment replacement, or carbon abatement.
---

# Retrofit Advisor: Building Decarbonization Planning

## Measure Hierarchy (Implement in This Order)

### Tier 1: No/Low Cost — Operational (0-6 months)
- Building tune-up / retro-commissioning: 5-15% energy savings, <1yr payback
- HVAC setback schedules: 3-8% savings, minimal cost
- Lighting occupancy sensors: 10-20% lighting savings, 2-3yr payback
- Leak detection (compressed air, steam): variable
- Metering and monitoring: enables targeted improvements

### Tier 2: Medium Investment — Systems (1-3 years)
- LED lighting retrofit: 40-60% lighting savings, 3-5yr payback
- Smart thermostats/BMS upgrade: 10-15% HVAC savings, 2-4yr payback
- Variable frequency drives (VFDs) on motors: 20-50% motor energy, 2-4yr payback
- Roof insulation improvement: 5-15% HVAC savings, 5-10yr payback
- Window film/glazing upgrade: 5-10% HVAC, 5-8yr payback

### Tier 3: Major Capital — Equipment Replacement (5-15 years)
- Chiller replacement (high-efficiency): 20-40% cooling savings, 7-12yr payback
- Boiler to heat pump conversion: 40-70% heating savings if electric grid clean, 8-15yr payback
- Cooling tower optimization: 10-20% cooling water, 5-8yr payback
- Solar PV installation: 20-40% electricity offset, 6-10yr payback (location-dependent)
- EV charging infrastructure: revenue-generating, regulatory compliance

## Carbon Abatement Cost Curve Framework

For each measure, calculate:
- **Annual energy savings** (kWh, therms, or MMBtu)
- **Annual CO2 reduction** (tCO2e) = energy savings × emission factor
- **Implementation cost** ($)
- **Annual cost savings** ($) = energy savings × utility rate
- **Simple payback** = cost / annual savings
- **Carbon abatement cost** ($/tCO2e) = net capex / lifetime CO2 reduction

Rank measures by: lowest carbon abatement cost first (carbon bang-for-buck)

## Hold-Period Alignment

Match retrofit investment horizon to asset hold period:
- **Hold <3 years:** operational measures only (retro-cx, tune-ups)
- **Hold 3-7 years:** Tier 1 + Tier 2 (lighting, controls, VFDs)
- **Hold 7-15 years:** All tiers including major equipment
- **Hold 15+ years:** Full electrification pathway

## Electrification Decision Framework

Should a building electrify HVAC?
1. Check local grid carbon intensity (lbs CO2/MWh) — electrification only helps if grid is <400 lbs/MWh
2. Assess current fuel type (gas vs. oil vs. electric)
3. Calculate all-in electrification cost (equipment + electrical upgrades)
4. Model energy cost impact (electricity vs. gas rates)
5. Calculate carbon reduction (vs. CRREM pathway)
6. Check utility incentives (IRA tax credits, utility rebates)

## IRA Tax Credits (US) — Key for ROI
- 179D Energy Efficient Commercial Buildings Deduction: $5/sf for achieving 50% energy reduction
- 48E Clean Electricity Investment Credit: 30% ITC for solar, storage, heat pumps
- 45L New Energy Efficient Home Credit: multifamily new construction
- Prevailing wage/apprenticeship: additional 20% multiplier

## Green Lease Clauses That Enable Retrofits
- Tenant data sharing (utility access)
- Cost recovery / green rent riders
- Landlord access for energy improvements
- HVAC maintenance standards
- Submetering requirements

## Required Output Format Per Recommendation

For each retrofit measure, provide:
- **Capex estimate** ($) and source/confidence level
- **Annual energy savings** (kWh/yr or GJ/yr) and **annual cost savings** ($/yr)
- **Simple payback period** (years = capex / annual savings)
- **IRR** if hold period > 5 years
- **Carbon abatement** (tCO2e/yr removed) and **abatement cost** ($/tCO2e = net capex / lifetime savings)
- **Hold-period alignment**: flag if payback > remaining hold period
- **Equipment remaining useful life** vs. replacement timing (don't replace 2-year-old equipment)
- **Regulatory urgency**: does BPS compliance deadline change the financial calculus?

## Measure Prioritization Framework

1. **Operational/behavioral** (lowest cost, fastest payback): lighting schedules, HVAC setpoint optimization, plug load management
2. **End-of-life replacement** (replace on failure with high-efficiency): upgrade when equipment reaches end of useful life
3. **Deep retrofit** (highest impact, longest payback): envelope upgrades, HVAC replacement, fuel switching, electrification

## Cross-References

- Use Audette carbon reduction plan for NPV analysis and measure interaction effects
- Use CRREM stranding year to determine urgency of decarbonization timeline
- Use BPS compliance deadlines to identify regulatory-driven capex windows

## Reporting Measures
For each recommended measure, report:
| Measure | Cost | Annual Savings | Payback | CO2 Reduction/yr | Abatement Cost | IRA Credit |
