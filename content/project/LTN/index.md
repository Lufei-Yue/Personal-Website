---
title: "Impact of Low Traffic Neighbourhoods on Traffic Accident in London "
authors:
- admin
date: "2024-08-16T00:00:00Z"
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
summary: How Effective are Low Traffic Neighbourhoods in Reducing Traffic Accidents? A City-Wide Difference-in-Differences Study in London. 

# tags:
# - Master Dissertation
# - Transport Policy
# - Python

featured: true

links:
# - name: Custom Link
#   url: http://example.org
# url_pdf: http://arxiv.org/pdf/1512.04133v1
url_code: 'https://github.com/LufeiYue1/DID-LTN-London'
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

## 1 Overview 

Low Traffic Neighbourhoods (LTNs) are urban planning interventions aimed at reducing through traffic and improving road safety for pedestrians and cyclists. This study evaluates the effectiveness of LTNs in reducing traffic accidents in London using a Difference-in-Differences (DID) approach. The study analyzes annual traffic accident data from 2015 to mid 2024 and employs both a classic DID model and an improved DID model to assess the short- and long-term effects of LTNs.

**🛠 Skills & Tools:** <kbd>Python</kbd> <kbd>Causal Inference</kbd> <kbd>Econometrics (DID)</kbd> <kbd>Spatial Analysis</kbd> <kbd>Data Visualization</kbd>

*Note: This work is currently being prepared for publication.*

![map](figure1.png)

---

## 2 Methodology

To quantify the impact, I constructed two econometric models (DID) to compare accident trends between LTN areas (treatment) and non-LTN areas (control).

**Model A: Classic DID** Captures the immediate impact of policy implementation.
$$
Y_{it} = \beta_0 + \beta_1 \cdot treatment_i + \beta_2 \cdot post_t + \beta_3 \cdot (treatment_i \times post_t) + \varepsilon
$$
![DID1](DID1.jpg)
**Figure 2.** Conceptual illustration of the classic DID model.

**Model B: Improved DID** Addressed unobserved heterogeneity and time-varying effects (e.g., the COVID-19 pandemic). The time trend terms was introduced to validate the **Parallel Trends Assumption** and separate short-term shocks from long-term safety improvements.
$$
\begin{aligned}
Y_{it} &= \beta_0 + \beta_1 \cdot \text{treatment}_i + \beta_2 \cdot \text{post}_t + \beta_3 \cdot (\text{treatment}_i \times \text{post}_t) \ + \\
&\quad \beta_4 \cdot \text{timebefore}_t + \beta_5 \cdot \text{timeafter}_t + \beta_6 \cdot (\text{treatment}_i \times \text{timebefore}_t) \ + \\
&\quad \beta_7 \cdot (\text{treatment}_i \times \text{timeafter}_t) + \varepsilon_{it}
\end{aligned}
$$
![DID](DID.jpg)
**Figure 3.** Conceptual illustration of the improved DID model.

---

## 3 Key Findings & Visualization 

💡**Insight 1: Diverging Trends**<br> While accident rates were similar prior to 2020, LTN areas showed a sustained decline post-implementation, whereas city-wide accidents rebounded after the pandemic.
![count](figure4.png)

💡**Insight 2: Borough-Level Heterogeneity**<br> Most boroughs exhibited a reduction in crashes. Areas with increased crashes typically had low baseline accident counts, indicating high variance but low absolute impact.
![change](figure5.png)

💡**Insight 3: Quantifiable Safety Improvement** <br>
Results confirm the safety benefits of LTNs:<br>
**Immediate Effect**: Classic DID showed a 26.5% reduction in accident log-counts ($coef = -0.3072$).<br>
**Long-term Effect**: The Improved DID model indicated a sustained 10.0% reduction ($coef = -0.2404$), proving the policy's lasting value beyond the pandemic anomaly.
![result1](result1.png)
![result2](result2.png)





<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
