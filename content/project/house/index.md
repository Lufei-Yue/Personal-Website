---
title: "California Housing Valuation: A Geo-XAI Approach"
authors:
- admin
date: "2025-12-26T00:00:00Z"
doi: ""
math: true

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
# publication_types: ["article"]

# # Publication name and optional abbreviated publication name.
# publication: ""
# publication_short: ""

# abstract: In this project, I investigated the causal impact of London's Low Traffic Neighbourhoods (LTNs) on road safety. Analyzing a decade of city-wide accident data, I used Python to employ an advanced Difference-in-Differences (DID) model to move beyond simple correlation. The analysis revealed a statistically significant and lasting 10% annual reduction in traffic crashes in areas with LTNs. These findings provide robust causal evidence that LTNs are an effective long-term strategy for improving urban safety, offering a critical data point for policymakers shaping future transport initiatives. 

# Summary. An optional shortened abstract.
summary: This project aims to build a robust valuation model for California real estate by fusing Geospatial Analysis with Machine Learning. Unlike traditional models that treat location merely as coordinates, this approach engineers spatial features (specifically proximity to the coastline) to capture the non-linear economic value of "location". 

# tags:
# - GIS
# - Machine Learning
# - Python

featured: true

links:
# - name: Custom Link
#   url: http://example.org
# url_pdf: http://arxiv.org/pdf/1512.04133v1
url_code: 'https://github.com/Lufei-Yue/California-Housing-Valuation-A-Geo-XAI-Approach'
# url_dataset: '#'
# url_poster: '#'
# url_project: ''
# url_slides: ''
# url_source: '#'
# url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# - internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

# California Housing Valuation: A Geo-XAI Approach
### Integrating GIS Feature Engineering with Explainable AI

## Overview

This project builds a robust real estate valuation model for the California housing market by fusing **Geospatial Analysis** with **Machine Learning**.

Unlike traditional models that treat coordinates merely as numbers, this approach engineers specific spatial features—specifically the **geodesic distance to the nearest coastline**—to capture the non-linear economic value of "location." Furthermore, the project moves beyond the "black box" of prediction by utilizing **SHAP (SHapley Additive exPlanations)** to visualize exactly how geography impacts price.

### Key Features
* **GIS Engineering:** Topology repair and coordinate reprojection (EPSG:4326 $\to$ EPSG:3310) for accurate meter-based distance calculations.
* **High-Performance ML:** Utilized **XGBoost** to capture complex, non-linear relationships, achieving an **$R^2$ score of ~0.82**.
* **Explainable AI (XAI):** Deployed SHAP values to quantify the marginal contribution of spatial features.
* **Interactive Visualization:** Generated a Folium heatmap to visualize the "Location Premium" (positive vs. negative spatial impact) across the state.

## Methodology

### 1. Data Acquisition & Cleaning
The dataset is sourced from the *Hands-On Machine Learning* repository. Initial steps involved handling missing values and preparing the raw dataframe.

### 2. GIS Feature Engineering
Raw Lat/Lon coordinates are insufficient for identifying "coastal proximity."
* **Reprojection:** Converted data to **California Albers (EPSG:3310)** to measure distance in meters rather than degrees.
* **Topology Repair:** Applied `.buffer(0)` to fix self-intersections in the California coastline polygon.
* **Calculation:** Computed the precise distance from every property to the nearest point on the coast.

### 3. Predictive Modeling
An **XGBoost Regressor** was trained on the enriched dataset.
* **Input Features:** Median Income, Housing Median Age, Rooms, Population, *Distance to Coast (Engineered)*, etc.
* **Performance:** The model achieved an $R^2$ of **0.8187** on the test set.

### 4. Explainable AI (SHAP)
We used TreeExplainer to calculate SHAP values, allowing us to see:
* **Global Importance:** Which features drive prices the most?
* **Local Interpretation:** How much does "being 5km from the coast" add to a specific house's value?

---

## Results & Visualisations

### 1. Feature Importance (SHAP Beeswarm)
The SHAP summary plot reveals that **Median Income** and **Distance to Coast** are the primary drivers of housing prices.
<img width="924" height="626" alt="image" src="https://github.com/user-attachments/assets/56456db0-6a1c-4ca7-bd89-0e2ba13422e7" />

### 2. The "Location Premium" Map
We visualised the spatial heterogeneity of housing value.
* **Red Areas:** Positive location premium (e.g., Coastal zones, Bay Area).
* **Blue Areas:** Negative location impact (e.g., Inland/Central Valley).
<img width="1770" height="1160" alt="image" src="https://github.com/user-attachments/assets/ac799c10-c08b-4e81-a75b-dff27db79c22" />

---


## 💡 Insights
* **Proximity Matters:** The engineered feature `dist_to_coast_km` proved to be a top-tier predictor, significantly improving model performance compared to using raw coordinates alone.
* **Non-Linearity:** The relationship between distance and price is not linear; prices drop sharply within the first 10-20km from the coast, which XGBoost captured effectively.






<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
