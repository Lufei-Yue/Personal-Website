---
title: "Solar Park Site Suitability Analysis: A Multi-Criteria Evaluation in Scotland"
authors:
- admin
date: "2024-01-17T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
# publication_types: ["article"]

# # Publication name and optional abbreviated publication name.
# publication: ""
# publication_short: ""

# abstract: For this project, I assumed the role of a GIS analyst tasked with identifying potential sites for a new solar park in Scotland. Using ArcGIS Pro, I developed a Multi-Criteria Evaluation (MCE) model to find the most suitable locations. The model integrated key factors like proximity to roads and built-up areas, low elevation, and south-facing slopes, while strictly excluding prime agricultural land. The final output was a comprehensive favorability map that clearly visualizes and ranks the most promising areas, providing a data-driven foundation for stakeholders to make informed decisions for future development. 

# Summary. An optional shortened abstract.
summary: Performed a site suitability analysis in ArcGIS Pro to identify optimal locations for a new solar park in Scotland. I used Multi-Criteria Evaluation (MCE) and raster analysis to combine factors like elevation, aspect, soil type, and proximity to infrastructure. The project culminated in a favorability map that provides a data-driven recommendation for stakeholders. 

# tags:
# - Master Project
# - GIS
# - Spacial Analysis
# - ArcGIS Pro

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
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---
**🛠 Skills & Tools:** <kbd>ArcGIS Pro</kbd> <kbd>Multi-Criteria Evaluation (MCE)</kbd> <kbd>Spatial Analysis</kbd> <kbd>Suitability Modelling</kbd> <kbd>Renewable Energy</kbd>

---

Scotland's rugged terrain and strict land-use regulations present unique challenges for renewable energy developers. The objective was to identify optimal locations that balance solar efficiency, infrastructure logistics and environmental preservation, rather than simply finding 'empty land'.

As a GIS Analyst, I was responsible for developing a data-driven model to identify the most commercially and environmentally viable sites for a new solar park across the entire region.

---

## The Multi-Criteria Evaluation (MCE)

To solve this spatial problem, I used ArcGIS Pro to create a weighted suitability model. This involved processing different datasets into a unified scoring system.

The analysis was driven by four critical spatial constraints:

* **Solar Efficiency (Aspect)**: south-facing slopes were prioritised to maximise solar insolation and energy generation potential.
* **Land preservation (constraint):** applied a Boolean mask to strictly exclude prime agricultural land, ensuring the project does not conflict with food security.
* **Logistical viability:** calculated Euclidean Distance to roads and built-up areas. Sites needed to be accessible for construction (close to infrastructure) but not intrusive to residential zones.
* **Topography (slope & elevation):** filtered for low elevation and flat terrain to minimise construction costs and engineering challenges.

---

## Result & Visualisation

These complex variables were synthesised into a single, easy-to-interpret visual output by performing a Weighted Overlay analysis.

The map below is the result of this spatial analysis. The resulting suitability surface transforms abstract data into a clear ranking system, with black areas indicating prime locations that meet all logistical and environmental criteria.

![Final Solar Suitability Map](map.jpg)
*Figure 1: The Final Suitability Map. The analysis effectively filtered out unsuitable terrain and highlighted high-potential zones (black areas), providing stakeholders with a data-driven foundation for land acquisition.*

### Impact
This workflow demonstrates a scalable solution for renewable energy planning. Automating the screening process enables stakeholders to:
1.  Reduce Risk by avoiding the purchase of land with hidden environmental or topographic constraints.
2.  Save time by instantly narrowing down thousands of square miles to a few dozen viable sites.
3.  Support decision-making by providing quantitative evidence for planning applications and investment committees.

<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
