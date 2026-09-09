# Energy Required to Pump Water to Kigali City

## Overview
This document analyzes the energy requirements for pumping water to Kigali City, Rwanda, focusing on the elevation difference between water sources and the city, and providing calculations for the electrical energy needed per cubic meter of water delivered.

## Key Elevation Data
- **Kigali City elevation**: 1,476 meters above sea level [Source: Elevation.maplogs.com]
- **Primary water source (Lake Mugesera/Karenge)**: 1,300 meters above sea level [Source: Wikipedia - Lake Mugesera]
- **Static elevation head**: 1,476 m - 1,300 m = **176 meters**

## Fundamental Physics of Water Pumping
The theoretical energy required to lift water is calculated using the formula:

**Energy (joules) = Volume (m³) × Density (kg/m³) × Gravity (m/s²) × Head (m)**

Where:
- Density of water = 1,000 kg/m³
- Gravity = 9.81 m/s²

To convert joules to kilowatt-hours (kWh):
**Energy (kWh) = Energy (joules) / 3,600,000**

Combining these, the theoretical energy per cubic meter per meter of head is:
**Energy (kWh/m³/m) = (1,000 × 9.81) / 3,600,000 = 0.002725 kWh/m³/m**

## Practical Energy Calculation (Including System Efficiency)
Real-world pumping systems have energy losses due to:
- Pump inefficiency (typically 60-85% efficient)
- Motor inefficiency (typically 85-95% efficient)
- Pipe friction losses
- Fitting and valve losses

The practical formula is:
**Energy (kWh/m³) = (Head in meters) / (367 × Overall Efficiency)**

Where 367 is derived from: 3,600,000 / (1,000 × 9.81) ≈ 367

Typical overall efficiency for water pumping systems (pump + motor + controls): **60-75%**

## Energy Calculation for Kigali's Static Head
Using Kigali's 176-meter static head:

### At 60% Overall Efficiency:
Energy = 176 / (367 × 0.60) = 176 / 220.2 = **0.80 kWh/m³**

### At 70% Overall Efficiency:
Energy = 176 / (367 × 0.70) = 176 / 256.9 = **0.68 kWh/m³**

### At 75% Overall Efficiency:
Energy = 176 / (367 × 0.75) = 176 / 275.25 = **0.64 kWh/m³**

## Additional Energy Components: Friction Losses
The static head calculation above only accounts for lifting water against gravity. Actual systems require additional energy to overcome:

1. **Pipe friction losses**: Depends on pipe length, diameter, material, and flow rate
2. **Fitting losses**: Elbows, valves, tees, etc.
3. **Entry/exit losses**: At intake and discharge points

For municipal water supply systems, friction losses typically add **20-50%** to the static head requirement, depending on:
- Distance from source to city
- Pipe diameter and condition
- Flow rate (higher flow = higher friction losses)
- System age and maintenance

### Estimated Total Head for Kigali System
Assuming moderate friction losses (30% additional head):
- Static head: 176 meters
- Friction losses: 176 × 0.30 = 53 meters
- **Total dynamic head**: ~229 meters

Revised energy calculation (at 70% efficiency):
Energy = 229 / (367 × 0.70) = 229 / 256.9 = **0.89 kWh/m³**

## Context: Water Consumption and Energy Implications
### Kigali's Water Demand
- Estimated daily water consumption: ~100,000 m³/day (varies by source and growth)
- Annual consumption: ~36.5 million m³/year

### Annual Electricity Requirement for Pumping
At 0.89 kWh/m³:
- Daily: 100,000 m³ × 0.89 kWh/m³ = **89,000 kWh/day**
- Annual: 36,500,000 m³ × 0.89 kWh/m³ = **32,485,000 kWh/year** (~32.5 GWh/year)

### Cost Implications
Using Rwanda's electricity tariff (~182 RWF/kWh or ~$0.16 USD/kWh):
- Daily pumping cost: 89,000 kWh × 182 RWF/kWh = **16,198,000 RWF/day** (~$14,240 USD/day)
- Annual pumping cost: 32,485,000 kWh × 182 RWF/kWh = **5,912,270,000 RWF/year** (~$5.2 million USD/year)

## Comparative Analysis
### Comparison to Other Cities
- **Johannesburg, South Africa**: ~0.4-0.6 kWh/m³ (lower elevation gain)
- **Denver, Colorado, USA**: ~0.3-0.5 kWh/m³ (Rocky Mountain foothills)
- **Mexico City**: ~0.8-1.2 kWh/m³ (significant elevation gain ~1,000m)
- **La Paz, Bolivia**: ~1.2-1.8 kWh/m³ (very high elevation ~3,600m)

Kigali's requirement of ~0.68-0.89 kWh/m³ reflects its moderate elevation gain of ~176m from Lake Mugesera.

### Comparison to Alternative Water Sources
If Kigali were to use sources at different elevations:
- **From Nyabarongo River (~1,350m)**: Head = 126m → ~0.49-0.64 kWh/m³
- **From deeper wells (~1,400m)**: Head = 76m → ~0.30-0.39 kWh/m³
- **From higher sources (~1,500m)**: Would require less pumping or could use gravity flow

## Optimization Opportunities
### 1. System Efficiency Improvements
- **High-efficiency pumps**: Modern pumps can reach 85-90% efficiency
- **Premium efficiency motors**: IE3/IE4 motors 92-96% efficient
- **Variable frequency drives (VFDs)**: Match pump speed to demand, saving 20-50% energy
- **Regular maintenance**: Clean impellers, aligned shafts, proper lubrication

### 2. Infrastructure Optimization
- **Pipe sizing**: Larger diameter reduces friction losses (higher CAPEX, lower OPEX)
- **Loop systems**: Reduce peak flows and friction losses
- **Leak detection and repair**: Reduce total volume needing pumping
- **Pressure management**: Reduce excess pressure in distribution network

### 3. Renewable Energy Integration
- **Solar PV pumping**: Excellent match for daytime water demand
- **Hydropower recovery**: Energy recovery from pressure reduction valves
- **Grid-tied systems with net metering**: Offset pumping costs with renewable generation

## Comparison with Solar PV Generation Potential
From the SOLAR_ROI_ANALYSIS in this repository:
- **100kW solar system** in Kigali generates ~148,920 kWh/year
- This could pump approximately: 148,920 kWh/year ÷ 0.89 kWh/m³ = **167,000 m³/year**
- Or about **457 m³/day** - roughly 0.46% of Kigali's estimated daily demand

### Solar-Powered Pumping Scenarios
- **1MW solar system**: Could pump ~4,570 m³/day (~4.6% of demand)
- **5MW solar system**: Could pump ~22,850 m³/day (~23% of demand)
- **10MW solar system**: Could pump ~45,700 m³/day (~46% of demand)

This demonstrates that solar PV could offset a significant portion of Kigali's water pumping energy requirements, particularly during daylight hours when both solar production and water demand peak.

## Recommendations for Kigali Water Supply
1. **Conduct detailed hydraulic modeling** to determine exact friction losses
2. **Implement energy audits** of existing pumping stations
3. **Prioritize high-efficiency equipment** in upgrades and replacements
4. **Consider solar PV integration** for daytime pumping operations
5. **Implement VFDs** on all major pumping stations
6. **Explore gravity-fed options** from higher elevation sources where feasible
7. **Monitor and benchmark** energy intensity (kWh/m³) regularly for continuous improvement

## Sources
1. Elevation of Kigali, Rwanda - MAPLOGS: https://elevation.maplogs.com/poi/kigali_rwanda.37590.html
2. Lake Mugesera elevation - Wikipedia: https://en.wikipedia.org/wiki/Lake_Mugesera
3. Karenge Drinking Water Supply System - Wikipedia: https://en.wikipedia.org/wiki/Karenge_Drinking_Water_Supply_System
4. Engineering ToolBox - Water Pumping Costs: https://www.engineeringtoolbox.com/water-pumping-costs-d_1527.html
5. Standard pumping energy calculation formulas (hydraulic engineering principles)

*Note: Actual energy consumption will vary based on specific system design, maintenance condition, flow rates, and local factors. The calculations above provide a reasonable engineering estimate for planning and analysis purposes.*

---

