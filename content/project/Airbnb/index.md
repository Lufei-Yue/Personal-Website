---
title: "London Airbnb Market Analysis"
authors:
- admin
date: "2026-01-06T00:00:00Z"
doi: ""
math: true

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
# publication_types: ["article"]

# # Publication name and optional abbreviated publication name.
# publication: ""
# publication_short: ""

# abstract: In this project, I investigated the causal impact of London's Low Traffic Neighbourhoods (LTNs) on road safety. Analyzing a decade of city-wide accident data, I used Python to employ an advanced Difference-in-Differences (DID) model to move beyond simple correlation. The analysis revealed a statistically significant and lasting 10% annual reduction in traffic crashes in areas with LTNs. These findings provide robust causal evidence that LTNs are an effective long-term strategy for improving urban safety, offering a critical data point for policymakers shaping future transport initiatives. 

# Summary. An optional shortened abstract.
summary: Spatial Data Science & Market Segmentation Strategy. 

# tags:
# - Spatial Data Science
# - Machine learning
# - Python

featured: true

links:
# - name: Custom Link
#   url: http://example.org
# url_pdf: http://arxiv.org/pdf/1512.04133v1
url_code: 'https://github.com/Lufei-Yue/London-Airbnb-Market-Analysis'
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
  preview_only: true

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

# London Airbnb Market Analysis
### Spatial Data Science & Market Segmentation Strategy

## Summary
This project utilises **spatial data science** and **unsupervised machine learning (K-Means)** to analyse the complex London short-term rental market. By processing real-world data from *Inside Airbnb*, the analysis identifies high-yield investment zones and segments the market into distinct operational personas, providing actionable insights for investors and policymakers.

## Key Business Problems Solved
1.  **Investment Strategy:** Identifying boroughs that offer the best balance between entry cost (price) and tourist demand (review volume).
2.  **Market Segmentation:** Moving beyond simple pricing to understand the distinct business models operating in London (e.g., "Occasional Sharers" vs "Commercial Hotels").

## Methodology & Tech Stack

### 1. Data Cleaning & Engineering
* **Raw Data Processing:** Handled dirty data (currency symbols, mixed types) using Regex and Pandas.
* **Outlier Removal:** Filtered extreme luxury assets (£1,000+) to focus on the mass market.
* **Standardisation:** Applied `StandardScaler` to normalise features for clustering algorithms.

### 2. Geospatial Analysis
* **Mapping:** Utilised **GeoPandas** and `contextily` to project listing data onto official London Borough boundaries (EPSG:3857).

* **Visualisation:** Created professional choropleth maps with optimised labelling strategies for dense urban areas.
<img width="1773" height="1589" alt="image" src="https://github.com/user-attachments/assets/25545fc2-8d31-43f2-9989-2b1247fac501" />
<img width="1056" height="706" alt="image" src="https://github.com/user-attachments/assets/d0b0c307-dbc3-4ea5-9c32-9f097d6aedac" />


### 3. Machine Learning (Clustering)
* **Algorithm:** K-Means Clustering.
* **Optimisation:** Used the **Elbow Method** to determine the optimal cluster count ($K=5$).
<img width="878" height="475" alt="image" src="https://github.com/user-attachments/assets/5a7e8fcf-a16e-4bc4-9f49-85bcb7432893" />


* **Interpretation:** Decoded mathematical clusters into business personas (e.g., *The Budget Kings*, *The Commercial Ops*).
<img width="1055" height="986" alt="image" src="https://github.com/user-attachments/assets/b7d9504a-a7bc-47eb-834a-be30c873e08b" />



## Key Insights & Visualisations

### The Investment "Sweet Spot"
While **Westminster** is the most expensive, boroughs like **Islington** and **Lambeth** showed the highest efficiency—moderate pricing with exceptional review engagement.

### Market Personas (The 5 Clusters)
The K-Means model identified five distinct operator types:
* **Cluster 0 (The Occasional Sharers):** Low availability (~88 days). Compliant with regulations.
* **Cluster 1 (The Commercial Ops):** High availability (~311 days). High regulatory risk.
* **Cluster 2 (The Budget Kings):** Low price (£103) but massive review volume. High turnover strategy.
* **Cluster 4 (The Long-Term Lets):** Extreme minimum nights (~274 days). Residential tenancies bypassing agents.




<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
