# Silverleaf Sunflower (*Helianthus argophyllus*) — Seed Yield Optimization Research

---

## Abstract

This report presents a mathematical optimization approach for maximizing sunflower seed yield based on spatial parameters and the golden ratio. Two populations of sunflowers with differing disc widths are simulated across identically sized 10m × 10m fields to determine the arrangement that maximizes seed packing and overall production.

---

## Table of Contents

1. [Introduction & Biology](#1-introduction--biology)
2. [Modelling](#2-modelling)
3. [Sensitivity Analysis](#3-sensitivity-analysis)
4. [Results](#4-results)
5. [Discussion](#5-discussion)
6. [Next Steps](#6-next-steps)
7. [Appendix](#7-appendix)
8. [References](#references)

---

## 1. Introduction & Biology

The sunflower species (*Helianthus annuus*) are members of the **Asteraceae** plant family, which comprises over 100 species of perennial and annual cultivated herbs native to North America.

*Helianthus argophyllus*, known as **Silverleaf sunflowers**, is a rare perennial herbaceous flower native to the coast of Texas. Key biological characteristics include:

- **Height:** 6–15 ft, multi-stemmed with silvery-green foliage
- **Harvest period:** May to June, lasting until end of August
- **Flowering heads:** Produces 1–5 per lifetime; heliotropic (rotates to face the sun)
- **Petals:** 10–15, yellow to orange

### Seeds & Florets

Silverleaf sunflowers produce a disc of mature **achene seeds** surrounded by petals, reaching up to 20 cm in diameter. Achenes are dry fruit seeds varying in colour — often dark with white stripes.

Floret arrangement is designed to maximize sun exposure and seed reproduction. Florets spiral from the center outward, each offset by the **golden angle**:

$$\phi = 360(2 - s) \approx 137.5°, \quad \text{where } s = \lim_{n \to \infty} \frac{F_n}{F_{n+2}} \approx 0.618$$

This means sunflower florets grow in increments determined by the golden ratio, producing the characteristic Fibonacci spiral pattern.

### Growth & Yield

- **Oil content:** 40–65% per achene seed
- **Protein content:** 20–40% per achene seed
- **Optimal temperature:** 25–30°C
- **Typical yield:** 28,000–75,000 seeds per hectare

**Growth cycle stages:** Germination → Vegetative → Reproduction → Flowering → Harvesting

Planting depth should be 1 to 1½ inches in well-drained soil. Broad row spacing is preferred — tight rows do not improve yield and restrict root/head development.

---

### Literature Review

Several prior studies using plant modelling algorithms inform this research:

- **Ding W.L. et al.** — Optimized spacing for maize, soybean, and rice using spatial organization and Photosynthetic Active Radiation (PAR). Found that broader spacing improved light distribution, fruit quality, and yield per unit area.

- **Quilot-Turion B. et al.** — Designed a virtual model to optimize peach tree parameters using genetic prototypes and virtual experiments to produce an ideal phenotype.

- **Kurt C. et al.** — Compared twin-row vs. single-row planting in peanuts. Twin-row planting doubled pod yield; lower plant density per unit area increased pods per plant.

---

### Mathematical Formulation & Modelling Overview

Two sunflower species are modelled across identically sized **10m × 10m** fields:

| Species | Max Disc Diameter |
|---------|-------------------|
| **Type A** | Up to 10 cm |
| **Type B** | 10–20 cm |

The golden ratio is used to determine how many seeds can be packed per disc diameter. Two alternative spatial layouts are tested to maximize the number of flowering heads per field.

---

## 2. Modelling

### 2.1 Spatial Parameters

*(Section to be completed — field layout diagrams and spacing calculations for Type A and Type B sunflowers across the 10m × 10m plots.)*

### 2.2 Life-cycle Survival Probability

*(Section to be completed — probabilistic model for seed survival across harvesting seasons based on regional location data.)*

---

## 3. Sensitivity Analysis

*(Section to be completed — analysis of how changes in spacing, disc width, and environmental constants affect seed yield output.)*

---

## 4. Results

*(Section to be completed — simulation outputs comparing seed yield across spatial configurations for Type A and Type B populations.)*

---

## 5. Discussion

*(Section to be completed — interpretation of results in the context of the golden ratio model and existing literature.)*

---

## 6. Next Steps

*(Section to be completed — proposed follow-up experiments, field validations, and model refinements.)*

---

## 7. Appendix

*(Supporting figures, raw data tables, and supplementary calculations.)*

---

## References

1. *Helianthus annuus (sunflower)*. (n.d.). CABI. https://www.cabi.org/isc/datasheet/26714

2. *Southern Exposure Seed Exchange — Silverleaf Sunflower*. (n.d.). https://www.southernexposure.com/products/silverleaf-sunflower/

3. *NatureServe Explorer 2.0 — Helianthus argophyllus*. (n.d.). https://explorer.natureserve.org/Taxon/ELEMENT_GLOBAL.2.147465/Helianthus_argophyllus

4. Sutton, C. (1992, April 17). Science: Sunflower spirals obey laws of mathematics. *New Scientist*. https://www.newscientist.com/article/mg13418173-200-science-sunflower-spirals-obey-laws-of-mathematics/

5. "Fibonacci Spirals in Plants." *SPIRALS1, Version 6*. http://homepages.math.uic.edu/~howard/spirals.html

6. Swinton, J., et al. (2016). Novel Fibonacci and Non-Fibonacci structure in the sunflower: Results of a citizen science experiment. *Royal Society Open Science*. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4892450/

7. Berglund, D. R. (2007). *Sunflower Production*. NDSU Extension Service.

8. Ding, W.L., et al. (2020). Optimization method to obtain appropriate spacing parameters for crop cultivation. *International Journal of Agricultural and Biological Engineering*. https://www.abepublishing.org/journals/index.php/ijabe/article/view/4877

9. Quilot-Turion, B., et al. Optimization of parameters of the 'Virtual Fruit' model to design peach genotype for sustainable production systems. *European Journal of Agronomy*. https://pubag.nal.usda.gov/catalog/562978

10. Kurt, C., et al. (2017). The effect of twin row planting pattern and plant population on yield and yield components of peanut (*Arachis hypogaea* L.). *Turkish Journal of Field Crops*. https://dergipark.org.tr/en/pub/tjfc/issue/37069/301768
