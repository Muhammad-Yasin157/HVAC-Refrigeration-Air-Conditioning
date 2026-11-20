<div align="center">
  <h2>HVAC System Design for a Corporate Office: Artistic Milliners Unit 15, Karachi</h2>
  <p><b>Complex Engineering Problem (CEP)</b></p>
</div>

| Field | Details |
| :--- | :--- |
| **Course** | ME-319 – Refrigeration & Air-Conditioning |
| **University** | NED University of Engineering & Technology, Karachi |
| **Project Type** | Complex Engineering Problem (CEP) |
| **Software** | Carrier HAP v4.90 \| Elite Software DuctSizer |
| **Location** | Artistic Milliners Unit 15, Karachi, Pakistan |
| **Submitted to** | Dr. Muhammad Anique Azam |

HVAC Design | Cooling Load Analysis | Duct Design | Energy Efficiency

</div>

---

## Table of Contents
1. [Overview](#overview)
2. [Key Results](#key-results)
3. [Building and Design Inputs](#building-and-design-inputs)
4. [Methodology](#methodology)
5. [Results in Detail](#results-in-detail)
6. [Energy Efficiency Improvements](#energy-efficiency-improvements)
7. [Environmental Impact](#environmental-impact)
8. [Repository Structure](#repository-structure)
9. [How to Use This Repository](#how-to-use-this-repository)
10. [Tools and Standards](#tools-and-standards)
11. [Team](#team)
12. [License](#license)
13. [Author](#author)

---

## Overview

This Complex Engineering Problem (CEP) presents a comprehensive HVAC system design for a three-zone corporate office building (25.5 m²) at Artistic Milliners Unit 15, Karachi. Following the ASHRAE methodology, cooling loads were calculated using the Hourly Analysis Program (HAP v4.90) and the duct network was designed and pressure-balanced using DuctSizer. The project achieves a peak cooling load of 18.7 kW (12.1 kW sensible) served by a Packaged Rooftop CAV/RH system at 808 L/s supply airflow, verified against ASHRAE 62.1-2022 for ventilation and IAQ compliance.

The work covers six tasks:

1. Building survey and scope definition
2. Cooling load calculation in Carrier **HAP v4.90**
3. Indoor air quality and thermal comfort check (**ASHRAE 62.1 / 55**)
4. Duct sizing and pressure balancing in **DuctSizer** (Elite Software)
5. Energy-efficiency improvements with quantified savings
6. Carbon-footprint assessment (GHG Protocol Scope 1 and 2)

The system is a **Packaged Rooftop unit, Constant Air Volume with Reheat (PKG ROOF, CAV/RH)** serving all three zones.

---

## Key Results

| Parameter | Value |
|---|---|
| Conditioned floor area | 25.5 m² (3 zones, 11 occupants) |
| Peak total cooling load | **18.7 kW (5.32 TR)** |
| Peak sensible load | 12.1 kW |
| Sensible Heat Ratio (SHR) | 0.648 |
| Peak load occurs | June, 16:00 (OA 37.0 °C DB / 27.7 °C WB) |
| Total supply airflow | 808 L/s (1,713 CFM) |
| Supply fan | 0.75 kW, 600 Pa |
| Outdoor air (ventilation) | 35 L/s (3.2 L/s per person), ASHRAE 62.1 compliant |
| Zone CO₂ | 708 to 721 ppm (limit 1,100 ppm) |
| Duct noise | NC 30 achieved vs NC 50 required |
| Energy saving (proposed upgrades) | **35.9 %** (7,652 kWh/yr) vs 3 % CEP minimum |
| Carbon reduction | **3,862 kg CO₂e/yr (36.4 %)** |

---

## Building and Design Inputs

| Zone | Space | Floor area | Occupants |
|---|---|---|---|
| Zone 1 | DGM Office | 9 m² | 5 |
| Zone 2 | Manager's Office | 8 m² | 3 |
| Zone 3 | Assistant Manager's Office | 8 m² | 3 |

**Envelope:** brick/concrete walls (U = 2.241 W/m²K, 54 m²), single-glazed windows and glass doors (U = 6.884 W/m²K, SC = 0.657), slab-on-grade floor, no direct roof exposure.

**Internal loads:** fluorescent lighting (280 W), task lighting (15 W), computers and printers (1,760 W), 11 occupants (office activity).

**Design conditions (Karachi, ASHRAE 169-2021):** summer 37.0 °C DB / 27.7 °C WB, winter 9.4 °C DB, indoor 24 °C cooling / 20 °C heating, operating hours 08:00 to 18:00.

---

## Methodology

```
Site survey ──► HAP v4.90 model ──► Peak load and airflow ──► DuctSizer (Equal Friction)
                     │                                              │
                     ▼                                              ▼
           ASHRAE 62.1 / 55 checks                    Pressure balance + NC noise check
                     │
                     ▼
        Energy upgrades ──► Carbon footprint (Scope 1 + 2)
```

- **Load calculation:** ASHRAE Transfer Function Method in HAP, 12-month hourly simulation, sizing on peak block load (ASHRAE 183).
- **Duct design:** Equal Friction method at 0.10 in.wg per 100 ft, rectangular galvanized steel, max velocity 900 FPM (trunk) / 500 FPM (runout).
- **Manual verification:** SHR, fan power, duct heat gain, TR conversion, sensible and latent coil load and bypass factor were re-calculated by hand and compared with HAP.

---

## Results in Detail

### Cooling coil (June 16:00)

| Parameter | Value |
|---|---|
| Entering DB / WB | 25.0 / 19.0 °C |
| Leaving DB / WB | 12.5 / 12.1 °C |
| Apparatus dew point | 11.2 °C |
| Bypass factor | 0.10 |
| Design supply temperature | 12.8 °C |
| Resulting space RH | 56 % |

### Zone design loads

| Zone | Sensible (W) | Latent (W) | Airflow (L/s) |
|---|---|---|---|
| Zone 1: DGM Office | 4,134 | 2,270 | 305 |
| Zone 2: Manager | 3,238 | 1,627 | 239 |
| Zone 3: Asst. Manager | 3,238 | 1,627 | 239 |

### Duct network

| Section | Size | Length | Airflow (CFM) | Velocity (FPM) |
|---|---|---|---|---|
| Trunk 1 | 18" × 18" | 11.5 ft | 1,713 | 785 |
| Trunk 2 | 16" × 14" | 9.5 ft | 1,142 | 818 |
| Runout 1 (Zone 1) | 13.5" × 13.5" | 8 ft | 571 | 478 |
| Runout 2 (Zone 2) | 13.5" × 13.5" | 8 ft | 571 | 478 |
| Runout 3 (Zone 3) | 13.5" × 13.5" | 16 ft | 571 | 478 |

Critical path: Runout 2, cumulative static loss 0.060 in.wg (14.9 Pa). Layout: Fan → Trunk 1 → Runout 1 and Trunk 2 → Runouts 2 and 3.

### Ventilation (ASHRAE 62.1-2022, Ventilation Rate Procedure)

Vbz = Rp·Pz + Ra·Az with Rp = 2.5 L/s·person and Ra = 0.3 L/s·m².
Zone 1 = 15.2 L/s, Zones 2 and 3 = 9.9 L/s each, **total = 35.0 L/s**, which equals the design outdoor airflow.

---

## Energy Efficiency Improvements

Existing system: aging R-22 rooftop unit (COP about 2.5), T8 fluorescent lighting, single-speed fan, no energy recovery.

| Improvement | Existing | Proposed | Saving (kW) | Annual kWh |
|---|---|---|---|---|
| Refrigerant retrofit R-22 to R-32 (COP 2.5 to 3.5) | 7.49 kW | 5.35 kW | 2.14 | 5,350 |
| LED lighting (280 W to 98 W) | 0.280 kW | 0.098 kW | 0.182 | 455 |
| VFD on supply fan (80 % speed) | 0.750 kW | 0.384 kW | 0.366 | 915 |
| ERV on 35 L/s outdoor air (70 % sensible) | n/a | n/a | 0.373 | 932 |
| **Total** | **21,300 kWh/yr** | **13,648 kWh/yr** | **2.69 kW** | **7,652 (35.9 %)** |

Assumptions: 2,500 operating hours per year, grid factor 0.489 kg CO₂/kWh (NEPRA 2023).

---

## Environmental Impact

Boundary follows the **GHG Protocol Corporate Standard** (GWP values from IPCC AR6).

| Scope | Existing (kg CO₂e/yr) | Proposed (kg CO₂e/yr) | Reduction |
|---|---|---|---|
| Scope 1: refrigerant leakage | 181 | 61 | 120 |
| Scope 2: electricity | 10,416 | 6,674 | 3,743 |
| **Total** | **10,597** | **6,735** | **3,862 (36.4 %)** |

Over a 10-year lifetime this avoids about **38.6 tonnes CO₂e**.

---

## Repository Structure

```
.
├── README.md
├── LICENSE
├── report/
│   └── ME319_CEP_Report.pdf               # Full CEP report
├── hap/
│   └── HAP_Reports_RAC_CEP2.pdf           # 34-page HAP output (loads, hourly, psychrometrics)
├── ductsizer/
│   ├── DuctSizer_Output_RAC_CEP.pdf       # Duct sizing, pressure and sound output
│   └── RAC_CEP_H.dsw                      # DuctSizer project file
├── drawings/
│   └── Floor_Plan_Zones.pdf               # Zone layout and duct routing
```

---

## How to Use This Repository

### How to Use This Repository

1. Read the full write-up in `report/ME319_CEP_Report.pdf`.
2. Check the raw software output and CAD layouts for any number or design detail in the report:
   - Loads, airflows, psychrometrics: `hap/`
   - Duct sizes, pressure losses, NC levels: `ductsizer/`
   - Zone layout and duct routing drawings: `drawings/Floor_Plan_Zones.pdf`
3. To reproduce the duct design, open `RAC_CEP_H.dsw` in Elite DuctSizer and use the inputs listed above.
---

## Tools and Standards

**Software:** Carrier HAP v4.90, Elite Software DuctSizer, AutoCAD.

**Standards and references:** ASHRAE 62.1-2022, 55-2020, 90.1-2022, 183-2007, 169-2021, ASHRAE Handbook (Fundamentals 2021, HVAC Applications 2019), SMACNA Duct Construction Standards, GHG Protocol (2015), IPCC AR6, NEPRA State of Industry Report 2023, Pakistan HCFC Phase-Out Management Plan.

---

## Team

| Name | Roll No. |
|---|---|
| Muhammad Yasin | ME-23157 |
| Muhammad Hussain | ME-23113 |
| Hamza Bin Anwar | ME-23115 |
| Inam Ullah | ME-23156 |

Department of Mechanical Engineering, NED University of Engineering & Technology, Karachi. Report date: 11 May 2026.

---

## License

Released for academic and educational reference. See [`LICENSE`](LICENSE) for terms. Building data belongs to the surveyed facility and is used here for coursework only.

## Author

Muhammad Yasin | Mechanical Engineering Student

- GitHub: [https://github.com/Muhammad-Yasin157](https://github.com/Muhammad-Yasin157)
- LinkedIn: [https://www.linkedin.com/in/muhammadyasin3648](https://www.linkedin.com/in/muhammadyasin3648)
- Email: [yasinbangash119@gmail.com](mailto:yasinbangash119@gmail.com)
