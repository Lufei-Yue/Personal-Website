---
title: "Geodemographic Classification for Social Impact: Targeting Youth Support in Leeds"
authors:
- admin
date: "2024-02-27T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
# publication_types: ["article"]

# # Publication name and optional abbreviated publication name.
# publication: ""
# publication_short: ""

# abstract: This project aimed to solve a real-world problem for the Leeds-based charity, Learning Partnerships. They needed to pinpoint neighbourhoods with the highest concentration of young, disadvantaged adults to effectively deploy a new support initiative. My goal was to transform raw census data into an actionable, location-based strategy for them. 
 

# Summary. An optional shortened abstract.
summary: To help the Leeds-based charity Learning Partnerships identify neighbourhoods with the highest concentration of young, disadvantaged adults. The aim was to create a data-driven map to guide their outreach and support services. 

# tags:
# - 
# - K-means clustering
# - ArcGIS Pro
# - SPSS

featured: true


links:
# - name: Custom Link
#   url: http://example.org
# url_pdf: http://arxiv.org/pdf/1512.04133v1
# url_code: 'https://github.com/LufeiYue1/DID-LTN-London'
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

**🛠 Skills & Tools:** <kbd>SPSS</kbd> <kbd>ArcGIS Pro</kbd> <kbd>Census Data Analysis</kbd> <kbd>Geodemographics</kbd> <kbd>Social Policy</kbd>

---

## 🎯 The Challenge: Precision Targeting for Social Aid

**Client:** Learning Partnerships (Leeds-based Charity)

In a time of limited resources, blanket approaches to social aid are inefficient. Learning Partnerships faced a critical operational challenge: they launched a support initiative for young, disadvantaged adults but lacked the granular data to know *exactly* where to deploy their teams. 

> **My Goal:** To transform raw census data into an **actionable, location-based strategy**, pinpointing neighbourhoods with the highest concentration of at-risk youth.

---

## 🔬 Methodology: Statistical Rigour

My approach moved from statistical abstraction to geographic reality. I selected key census variables acting as proxies for disadvantage (e.g., unemployment, educational attainment) and applied the **K-means clustering algorithm** in **SPSS**.

### 1. Model Validation
Before interpreting the results, it was crucial to ensure the statistical validity of the segmentation. 

The boxplot below (Figure 1) illustrates the distance of cases from their respective classification clusters. The relatively tight distribution, particularly among our target groups, confirms that the mathematical clusters are cohesive and that the model has successfully grouped the diverse neighbourhoods together in a meaningful way.

![Data Processing and Methodology](1.png)
*Figure 1: Box plot showing the distance of cases from cluster centers. The analysis confirms the statistical distinctiveness of the four generated groups.*

---

## 📊 Key Insights: Identifying the "Target Group"

The clustering process revealed four distinct demographic profiles. Upon analysing the Z-scores of the variables (see Figure 2), one specific group **Cluster 3** stood out immediately as the primary target for the charity.

### 🏷️ Profile: The "Multilingual Multicultural Unemployment" Cluster

As shown in the bar chart below, **Cluster 3** (the tall bars in the middle) exhibits a drastic deviation from the average:
* **Highest Unemployment:** The teal bar shows a massive spike in unemployment among 16-74 year olds.
* **Language Barriers:** The light blue bar indicates a high percentage of residents who cannot speak English well.
* **Young Demographics:** Significant density of persons aged 25-44.

![Cluster Profile Analysis](CLuster.png)
*Figure 2: Final Cluster Centers (Z-scores). Note how Cluster 3 (Third group) shows significantly higher values for unemployment and non-English speaking variables compared to other groups.*

---

## 🌍 Impact: From Data to Strategy

The final step was to bring these statistics to life using **ArcGIS Pro**. By joining the classification data to Leeds' geographic boundaries, I produced a clear, visual map for the charity's stakeholders.

The map confirms that the target group (**Cluster 3**, represented in **Dark Brown**) is not randomly scattered. Instead, it forms a solid, actionable zone concentrated in **inner-city Leeds**.

![Final Suitability Map](map.jpg)
*Figure 3: Geodemographic Classification Map of Leeds. The Dark Brown areas represent the "Multilingual Multicultural Unemployment" cluster - the high-priority zones for Learning Partnerships' intervention.*

### 🚀 Outcome
This project provided Learning Partnerships with a robust **evidence base**. 
* **Strategic Focus:** The charity shifted from a city-wide approach to a targeted campaign in the inner-city "Dark Brown" zones.
* **Tailored Service:** Understanding the "Multilingual" nature of Cluster 3 allowed them to recruit staff with relevant language skills.
* **Social Impact:** Resources were successfully redirected to the communities with the most acute needs.


<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
