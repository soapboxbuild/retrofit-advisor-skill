# Retrofit Advisor Skill

AI-ranked building retrofit recommendations with ROI, payback period, energy savings, and carbon reduction analysis.

## What It Does

The Retrofit Advisor skill helps real estate owners, asset managers, and sustainability teams plan building decarbonization investments. It generates prioritized capex roadmaps aligned to hold period, budget, and carbon targets.

## Commands

### `/recommend`
Generate ranked retrofit recommendations with ROI and carbon impact for a building. Covers all three tiers: operational measures, systems upgrades, and major equipment replacement.

### `/electrification`
Evaluate the economics of electrifying HVAC — heat pumps, grid carbon intensity, IRA 48E credits, adjusted payback and IRR.

### `/capex-plan`
Build a multi-year decarbonization capex plan phased against compliance deadlines (BEPS, CRREM pathways), with year-by-year cost and carbon projections.

## Key Features

- **Tiered measure hierarchy** — operational (0-6 months) through major capital (5-15 years)
- **Carbon abatement cost curves** — rank measures by $/tCO2e for maximum carbon bang-for-buck
- **Hold-period alignment** — match investment horizon to asset strategy
- **IRA tax credit integration** — 179D, 48E, 45L credits factored into ROI
- **CRREM pathway alignment** — check stranding risk and compliance trajectory

## Installation

```bash
npx skills add soapboxbuild/retrofit-advisor-skill
```

Or install via Claude Code plugins from `https://github.com/soapboxbuild/retrofit-advisor-skill`.

## License

Apache-2.0 — Soapbox (https://soapbox.build)
