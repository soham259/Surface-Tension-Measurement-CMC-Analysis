# 🧪 Surface Tension Measurement & CMC Analysis
### Capillary Rise Method · Distilled Water · Vegetable Oil · Aqueous SLS

![Course](https://img.shields.io/badge/ChE--314-Colloids_%26_Interfaces-blue?style=flat-square)
![Method](https://img.shields.io/badge/Method-Capillary_Rise-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)
![Institute](https://img.shields.io/badge/IIT-Indore-red?style=flat-square)

---

## 📌 Overview

This project measures the **surface tension of three liquid systems** — distilled water, vegetable oil, and aqueous Sodium Lauryl Sulphate (SLS) — using the **capillary rise method**, and interprets the surfactant result within the **Critical Micelle Concentration (CMC)** framework.

| Liquid | σ (N/m) | Bond Number | vs. Literature |
|---|---|---|---|
| Distilled Water | **0.07106** | 0.0225 | 1.3% from 0.072 N/m ✅ |
| SLS + Water | **0.04232** | 0.0378 | At/just above CMC |
| Vegetable Oil | **0.02937** | 0.0491 | — |

> **Key result:** σ ordering confirmed — Water > SLS > Oil. SLS identified at or just above CMC with **40.5% surface tension reduction** from water baseline.

---

## 🔬 Background

**Surface tension** arises from the net inward pull on molecules at a liquid surface. It is defined as:

```
σ = F/L = dW/dA      [N/m = J/m²]
```

**Critical Micelle Concentration (CMC):** The threshold surfactant concentration beyond which the air-water interface is fully saturated and additional surfactant self-assembles into bulk micelles. σ stops falling at the CMC.

| Regime | Behaviour |
|---|---|
| Below CMC | σ drops as surfactant crowds the interface |
| At CMC | Interface saturated, σ at minimum |
| Above CMC | Micelles form in bulk, σ stays flat |

---

## ⚙️ Methodology

### Governing Equation

Force balance on the liquid column in a capillary of radius *r*:

```
F↑ = σ · 2πr · cos θ      (surface tension)
F↓ = ρ · g · h · πr²     (weight of column)

Setting F↑ = F↓ with cos θ ≈ 1:
σ = ½ · ρ · g · h · r
```

### Supporting Diagnostics

| Diagnostic | Formula | Purpose |
|---|---|---|
| Jurin–da Vinci Constant | r·h = 2σ/ρg | Internal consistency check |
| Capillary Length | a = √(2σ/ρg) | Surface tension vs gravity length scale |
| Bond Number | Bo = (r/a)² | Validates capillary formula (need Bo ≪ 1) |

### Procedure
1. Clean and dry capillary tube (I.D. = 1.1–1.2 mm)
2. Mount vertically, lower tip to liquid surface
3. Wait ~20 seconds for meniscus equilibrium
4. Withdraw and measure rise height
5. Repeat 6 times across 3 sample volumes per liquid

---

## 📊 Results

<img width="1280" height="960" alt="image" src="https://github.com/user-attachments/assets/c2003ace-768e-4ea0-9d62-8df33d1a23fb" />


### Raw Observations

| Liquid | Mean Rise Height (cm) | σ (N/m) |
|---|---|---|
| Distilled Water | 2.550 | 0.07106 |
| SLS + Water | 1.517 | 0.04232 |
| Vegetable Oil | 1.167 | 0.02937 |

### Validation

All Bond numbers well below 0.05 threshold — simple capillary formula valid:

| Liquid | Bo | Capillary Length a (mm) | r·h (m²) |
|---|---|---|---|
| Water | 0.0225 | 3.804 | 1.454 × 10⁻⁵ |
| SLS | 0.0378 | 2.934 | 0.865 × 10⁻⁵ |
| Oil | 0.0491 | 2.572 | 0.665 × 10⁻⁵ |

### CMC Analysis

```
Δσ = σ_water − σ_SLS = 0.07106 − 0.04232 = 0.02874 N/m
Relative reduction = 40.5%
```

SLS solution at **σ = 0.04232 N/m** is only **1.06×** above the literature CMC plateau (0.035–0.040 N/m) — confirming the solution is **at or just above CMC** with a nearly saturated air-water interface.

### Error Analysis

| Liquid | σ (N/m) | Δσ (N/m) | Relative Error |
|---|---|---|---|
| Water | 0.07106 | ±0.00051 | <1% |
| Oil | 0.02937 | ±0.00053 | <2% |
| SLS | 0.04232 | ±0.00072 | <2% |

---

## 📁 Repository Structure

```
📦 Surface-Tension-CMC-Analysis/
├── 📄 README.md
├── 📂 Report/
│   └── Stage3_SurfaceTension_CMC_Report.pdf
└── 📂 Presentation/
    └── Stage3_SurfaceTension_CMC_pptx.pdf
```

## 🎞️ Presentation

📊 View the full slide deck here: **[Canva Presentation](https://canva.link/z5chyabe5op1srt)**

---

## 🔑 Key Conclusions

1. **σ ordering validated** — Water (0.07106) > SLS (0.04232) > Oil (0.02937) N/m, consistent with H-bonding, amphiphilic adsorption, and non-polar cohesion respectively.
2. **Distilled water within 1.3% of literature** (0.072 N/m at 30°C) — confirms removal of mineral contamination vs. tap water.
3. **All Bond numbers < 0.05** — capillary formula valid across all three systems, no meniscus distortion.
4. **< 2% relative uncertainty** on all σ values from propagated error analysis.
5. **SLS at CMC** — 40.5% reduction from water baseline places solution at onset of bulk micelle formation.

---

## 👥 Team

| Member | Contribution |
|---|---|
| Soham Raut | Calculations, experiments, content review |
| Adya Singh Bishain | Experiments, initial calculations, literature review |
| Mannan Mahajan | Experiments, calculations, report & presentations |
| Samarth Sharma | Calculations, error propagation, data visualization |
| Abhinav Singh | Filming, editing, voice-over |

**Course:** ChE-314 Colloids & Interfaces | Stage 3 Final Evaluation  
**Institution:** Indian Institute of Technology Indore | April 2026

---

## 📚 References

1. Berg, J. C. (2010). *An Introduction to Interfaces and Colloids.* World Scientific.
2. Adamson & Gast (1997). *Physical Chemistry of Surfaces*, 6th ed. Wiley.
3. Rumble, J. R. (2024). *CRC Handbook of Chemistry and Physics*, 105th ed.
4. Rosen & Kunjappu (2012). *Surfactants and Interfacial Phenomena*, 4th ed. Wiley.
5. Vella & Mahadevan (2005). The "Cheerios effect." *Am. J. Physics*, 73(9).
