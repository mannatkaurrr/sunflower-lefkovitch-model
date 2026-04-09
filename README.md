# Maximizing Silverleaf Sunflower Seed Production (Maple)

**Mannat Kaur**  
**MATH 3052 - Mathematical Biology - York University**  
**Professor Heffernan**

---

## Project Highlights

- Built a Lefkovitch age-structured population model for Silverleaf sunflowers
- Compared two planting configurations under equal land area
- Applied eigenvalue analysis to evaluate long-term population stability
- Simulated two growing seasons using Maple
- Quantified how spatial design impacts viable seed production

## Impact

This project demonstrates how mathematical biology and eigenvalue analysis can guide real resource decisions such as crop layout and conservation planning. The workflow mirrors industry forecasting: define assumptions → build model → validate → deliver decision insight.

## Skills

- Mathematical Biology
- Matrix Algebra
- Eigenvalue Analysis
- Lefkovitch Model
- Maple
- Scientific Computing & Modelling

## Table of Contents

- [Problem Context](#problem-context)
- [Data & Assumptions](#data--assumptions)
- [Methodology](#methodology)
- [Results](#results)
- [Full Report](#full-report)
- [Full Maple Code](#full-maple-code)

---

## Problem Context

I developed a quantitative model to evaluate how spatial planting design affects long-term seed production of Silverleaf sunflowers, a slow-growing perennial species. The goal was to compare two field strategies (10 cm vs 20 cm flower heads) on identical land area and determine which configuration maximizes viable offspring using age-structured population dynamics.

---

## Data & Assumptions

Inputs included disc diameter, golden-ratio floret formula, and survival transitions between six life stages (seed → 5-headed sunflower). Environmental factors were held constant to isolate spatial effects.

### Field Layout Comparison

<p align="center">
  <img src="images/sunflower-field-a.png" width="420">
  <img src="images/sunflower-field-b.png" width="420">
</p>

<p align="center"><em>Figure 1. Comparison of sunflower field layouts for Population A (10 cm heads) and Population B (20 cm heads) under equal land area.</em></p>

---

## Methodology

- Estimated achene seeds per head using **φ = 0.618**
- Constructed Lefkovitch matrices with progression, regression, and fertility terms
- Evaluated dominant eigenvalue **λ** to assess population stability
- Simulated two seasons in Maple

### Seed Density Modelling

<p align="center">
  <img src="images/seed-density-a.png" width="420">
  <img src="images/seed-density-b.png" width="420">
</p>

<p align="center"><em>Figure 2. Estimated maximum achene seed density for Population A and Population B using golden-ratio-based disc modelling.</em></p>

### Life-Cycle Structure

<p align="center">
  <img src="images/lifecycle-diagram.png" width="550">
</p>

<p align="center"><em>Figure 3. Life-cycle transition structure used to define stage progression, regression, and fertility in the Lefkovitch population model.</em></p>

---

## Results

- **Population A (10 cm):** 557,857 seeds after 2 seasons  
- **Population B (20 cm):** 1,653,473 seeds after 2 seasons  
- **λA = 87.77**  
- **λB = 147.47**

**Insight:**  
Larger head diameter produced approximately **3× more seeds** despite equal surface area, demonstrating that wider spatial design significantly improves reproductive output and long-term population growth.

---

## Full Report

**[View Final Report PDF](silverleaf-sunflower-report.pdf)**

---

## Full Maple Code

**[View Maple Code](maple-code.md)**

---
