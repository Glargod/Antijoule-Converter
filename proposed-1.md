# Phase 1 Proposal: Testing Geometric Enhancement in Ni-63 Betavoltaic Collectors  
**Open-Source, Low-Risk Exploration of Coherence / Reflection Effects**  
**Version 1.0 — March 2026**  
**Inspired by Antijoule Converter concepts (glargod.github.io/Antijoule-Converter/)**

## 1. Objective  
Construct and compare two sealed betavoltaic collectors using Ni-63:  
- **Control**: standard flat geometry (baseline betavoltaic performance)  
- **Test Vessel**: shaped (parabolic / pyramidal / reflective cavity) to encourage longer paths, coincidental returns, or mild angle biasing of low-energy betas  

Measure sustained electrical output (voltage, current, cumulative charge) over ≥6–12 months.  
Seek any persistent, statistically significant excess in the test vessel that exceeds expectations from geometry/reflection alone (Monte Carlo modeled).  
**No over-unity or free-energy claims intended** — only honest data to bound or support subtle "antijoule"-like effects (pre-paid barrier energy harvest via gentle loop / resonance).

## 2. Rationale & Expected Baseline  
Ni-63: pure β⁻ emitter, t½ ≈ 100.2 y, E_max ≈ 67 keV, E_avg ≈ 17–18 keV.  
Typical betavoltaic performance (literature):  
- Power density \~1–10 nW/cm² (often 2–3 nW/cm² reported)  
- Energy conversion efficiency \~0.5–3% (up to \~6–8% in optimized Si/GaAs/SiC setups)  
- Dominant losses: self-absorption in source, random emission directions, backscatter, recombination  

Hypothesis: Vessel geometry (reflective inner surfaces, converging apex to collector) could increase effective collection by guiding strays, increasing path length, or enabling coincidental feedback → measurable ΔP > baseline (target: ≥20–30% sustained excess after uncertainty subtraction).

## 3. Materials (Minimal & Replicable)  
- **Radioisotope Source**  
  - Ni-63 foil or electroplated layer, 1–5 mCi total activity (\~1 cm² area, few μm thick)  
  - Specific activity \~10 Ci/g or better; source certified & licensed  
- **Vessel / Collector Structures** (two identical except geometry)  
  - Material: copper or tungsten base, gold-plated or lined  
  - Inner reflector: thin low-Z layer (beryllium, diamond-like carbon, or similar for elastic β scatter at \~17 keV)  
  - Control: flat plate geometry  
  - Test: parabolic bowl or shallow pyramid (\~1–2 cm³ volume), apex opening to collector  
  - Optional resonance: micro-coil or cavity tuned near beta spectrum (exploratory)  
- **Semiconductor Collector**  
  - Si PIN diode, GaAs Schottky, or SiC junction (\~1 cm² active area)  
  - Optional bias network (low-power)  
- **Sealing & Logging**  
  - Vacuum or inert-gas epoxy/glass enclosure  
  - Low-power electronics: LTC3108-style harvester + tiny MCU (e.g. ATTiny) logging to SD or e-ink display  
  - Cumulative charge counter visible externally (LCD/e-ink powered by device itself)  

## 4. Safety & Regulatory Notes  
- <10 mCi → typically exempt quantity (verify CNSC / local regs for Canada)  
- Shielding: 1–2 mm Cu/plastic stops betas completely  
- Handling: glovebox assembly, wipe tests, licensed source supplier  
- Disposal: return source or certified rad-waste protocol  

## 5. Experimental Protocol  
1. Fabricate two matched sets (control + vessel) with identical Ni-63 activity  
2. Calibrate electronics; baseline dark current / noise  
3. Seal both devices identically; reset timers/counters at t=0  
4. Store in dark, temperature-controlled enclosure (20 ± 2 °C)  
5. Monitor:  
   - Weekly: V_oc, I_sc, power, cumulative charge  
   - Continuous logging if possible (temperature, humidity, background)  
6. Duration: ≥6–12 months (Ni-63 decay negligible)  
7. Analysis: compare vessel vs control; subtract modeled geometric gain (use GEANT4 / MCNP for reflection/backscatter estimate)  

## 6. Success / Anomaly Criteria  
- **Null / Expected**: vessel ≈ control (±10–15% after uncertainty)  
- **Positive Signal**: vessel shows ≥20–30% sustained higher power (p<0.05 over months), unexplained by reflection model  
- **Strong Anomaly**: output rises over time, or decay appears suppressed → halt, replicate independently, calorimetry  
- **Failure Modes**: vessel lower (absorption issue) → iterate reflector / shape  

## 7. Open-Source Commitment  
- Full BOM, CAD/STL files, assembly guide, code on GitHub repo  
- Raw data uploaded periodically (anonymous if desired)  
- Invite makers, labs, universities to replicate / vary geometry  

## 8. Risks & Conservatism  
- Power remains nanowatts — proof-of-concept only  
- Physics laws hold unless data demands reevaluation  
- Null result bounds accessibility of "antijoule" effects  

## 9. Potential Phase 2 (If Positive)  
- Shorter t½ isotopes (Pm-147, etc.)  
- Active resonance tuning  
- Higher-density sources (speculative Th-232 traces)  

**Build small. Measure honestly. Share openly.**  
**Let the numbers whisper what they will.**
