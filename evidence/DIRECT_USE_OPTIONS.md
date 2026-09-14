# Direct Use Options for Rwandan Geothermal Heat

## Overview

This document assesses what Rwanda's *currently measured* geothermal resource can support, and explains why direct thermal use is the venture's entry point rather than electrical generation. It is the evidence base for Phase 2 of the business plan.

The conclusion is that direct use is technically supportable today on the confirmed Gisenyi spring, while power generation is not — and that the commercial case for direct use rests on assumptions about customers that are **not yet verified**.

Figures are tagged throughout:

- **[Measured]** — observed and sourced.
- **[Benchmarked]** — taken from a cited analogue, not from Rwanda.
- **[ASSUMED — VERIFY]** — no source. Must be confirmed before any investment decision.

## The Resource Constraint

The only measured geothermal temperature in Rwanda's public record is the **Gisenyi hot spring at 70–75°C [Measured]** (see `GEOTHERMAL_RESOURCE_BASE.md`). No flow rate has been published for it or for any other Rwandan spring.

That 70–75°C figure matters in two directions:

- It is **too low to be interesting for power**. A 75°C resource driving a brine temperature drop of ~30 K at roughly 5% net conversion efficiency needs on the order of 150 kg/s of fluid per megawatt electrical. No Rwandan spring is documented to produce anything close to that.
- It is **well matched to heat**. At 70–90% thermal efficiency, the same fluid produces usable heat directly, and 75°C is a good match for the greenhouse, aquaculture and low-temperature process heat duties described below.

This is the arithmetic behind the phase order in the business plan. It is not a preference for simpler technology; it is what the measured resource supports.

## Why Direct Use Is the Entry Point

| Metric | Electrical Generation | Direct Thermal Use |
|---|---|---|
| Conversion efficiency | 10–15% **[Benchmarked]** | 70–90% **[Benchmarked]** |
| Capital cost per useful kW | $2,500–$4,000/kWe **[Benchmarked]** | $500–$1,500/kWt **[Benchmarked]** |
| Technical complexity | High — power conversion, grid connection | Low to medium — heat exchangers, pumps |
| Requires drilled resource | Yes | **No** — works on the measured spring |

The capital cost figures are benchmark ranges for the technology class, not Rwandan quotations. No Rwandan supplier pricing exists in any public source.

A further advantage is that direct use creates no offtake dependency on the national grid, and therefore does not require a RURA generation licence or a PPA to begin generating revenue (see `../REGULATORY_AND_OFFTAKE.md`).

## Option 1: Greenhouse Heating

**Temperature match.** 70–75°C is well suited to greenhouse heating duties. **[Benchmarked]**

**What it displaces.** The commercial case assumes displacement of diesel or biomass heating fuels, valued at an effective ~$0.15/kWh thermal. **[ASSUMED — VERIFY]** This is the single most fragile number in the direct-use case — see *The Counterfactual Problem* below.

**Worked example as originally calculated.** A 500 kW thermal system running 8,000 hours per year at 75% delivery efficiency:

- Thermal energy delivered: 500 kW × 8,000 h × 0.75 = **3,000,000 kWh thermal/year** **[Benchmarked]**
- Diesel displaced at 10 kWh thermal/litre: **300,000 litres/year** **[ASSUMED — VERIFY]**
- Value at 1,700 RWF/litre: **510,000,000 RWF/year (~$443,000 USD/year)** **[ASSUMED — VERIFY]**

The 0.5–1.5 year simple payback that appeared in the earlier repository analysis derives from this chain and ignores the customer risk described below. **It should not be relied on.** No such customer has been identified, and no heat supply agreement has been discussed.

**What would need to be true:** a greenhouse operator within economic pumping distance of the spring, currently paying for diesel or biomass heat, with year-round demand and the balance sheet to sign a 10–15 year heat supply agreement.

## Option 2: Aquaculture

**Temperature match.** Tilapia perform best at 28–30°C, so 70–75°C source water requires mixing and temperature control rather than direct use. **[Benchmarked]** This is a real engineering constraint, not a formality — it adds a mixing and control system to the capital cost.

**Advantages.** Year-round production, faster growth, reduced disease incidence, and access to both domestic and export protein markets.

**Assessment.** Plausible but weaker than greenhouse heating on temperature match, and it depends on a fish-farming sector of sufficient scale near the prospect. That sector's size and current energy spend are **not established** in any source reviewed. **[ASSUMED — VERIFY]**

## Option 3: Industrial Process Heat

**Target sectors.** Food processing (pasteurisation, drying, sterilisation), textiles (dyeing, drying), breweries (mashing, wort boiling) and dairy (pasteurisation) all operate in the 70–75°C band or below.

**Assessment.** Potentially the largest and most creditworthy customer class, because industrial heat demand is continuous, metered and already purchased commercially. It is also the slowest to convert, since it requires retrofitting an existing process heat system and negotiating with a commercial counterparty.

The population of suitable industrial facilities near Gisenyi or Bugarama has **not been surveyed**. This survey is a Phase 1 deliverable in the implementation plan, not an established fact. **[ASSUMED — VERIFY]**

## Option 4: Geothermal-Assisted Heat Pumps

**Concept.** Use geothermal fluid as the source or sink for high-efficiency heat pumps serving municipal water facilities, reducing the electrical energy needed to pump and treat water.

**Context.** Kigali's water pumping load was estimated in the archived `WATER_PUMPING_ENERGY.md` at roughly 32.5 GWh/year and ~$5.2 million/year. Those figures are **archived and unverified** and are cited here only to indicate the scale of the municipal load, not as a revenue line.

**Assessment.** This is a municipal infrastructure proposition requiring a utility counterparty, not a private heat sale. It is a longer-horizon option and is not part of Phase 2.

## Ranking

| Rank | Option | Temperature fit | Customer identified? | Phase |
|---|---|---|---|---|
| 1 | Greenhouse heating | Good | **No** | Phase 2 |
| 2 | Industrial process heat | Good | **No** | Phase 2 |
| 3 | Aquaculture | Requires mixing | **No** | Phase 2–3 |
| 4 | Heat pumps for water facilities | Indirect | Municipal utility | Phase 3+ |

## The Counterfactual Problem

This is the most important caveat in the document.

The direct-use case values delivered heat at the cost of the fuel it displaces. That is only valid if the customer **actually burns that fuel today**. If the prospective customer instead uses grid electricity, biomass, or has no existing heat demand at all, the avoided cost is materially lower — in the biomass case, potentially an order of magnitude lower.

At present:

- No customer has been identified.
- No customer's current fuel and energy spend has been audited.
- No heat sale price has been agreed.

Until those three things are established, **the direct-use revenue case is unproven**, and the plan treats it as such. The 0.5–1.5 year payback quoted in earlier repository analysis is an arithmetic result, not a forecast, and it is the mirror image of the same defect that made the electrical payback figures unusable.

## What Must Be Verified Before Investment

1. **Measured flow rate** at the Gisenyi spring, in litres per second, with seasonal variation. Without this, the size of any direct-use system is unknown. This is a Phase 1 deliverable.
2. **Named target customers**, with audited current energy spend and fuel type.
3. **A heat supply agreement term sheet** with at least one customer, covering price, tenure and volume.
4. **Rwandan equipment and installation pricing**, replacing the benchmark capital cost ranges.
5. **Water rights and discharge arrangements** for fluid extraction and reinjection, confirmed with the relevant authorities.

## Sources

1. [Rwanda Energy Group - Geothermal Section](https://www.reg.rw/what-we-do/generation/geothermal/)
2. [UNIDO Geothermal Fact Sheet for Rwanda (PDF)](https://downloads.unido.org/ot/32/09/32096187/Geothermal%20fact%20sheet%20for%20promoting%20PPP%20-Rwanda.pdf)

*Note: Capital cost and efficiency ranges are international benchmarks for the relevant technology classes, not Rwandan quotations. Direct-use revenue figures carried forward from earlier repository analysis are marked as unverified and should not be relied upon.*

---
