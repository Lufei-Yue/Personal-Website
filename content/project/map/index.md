---
title: "Spatial Analysis and Cartography: Creating China's Annual Precipitation Distribution Map"
authors:
- admin
date: "2020-09-12T00:00:00Z"
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

# abstract: In this project, I investigated the causal impact of London's Low Traffic Neighbourhoods (LTNs) on road safety. Analyzing a decade of city-wide accident data, I used Python to employ an advanced Difference-in-Differences (DID) model to move beyond simple correlation. The analysis revealed a statistically significant and lasting 10% annual reduction in traffic crashes in areas with LTNs. These findings provide robust causal evidence that LTNs are an effective long-term strategy for improving urban safety, offering a critical data point for policymakers shaping future transport initiatives. 

# Summary. An optional shortened abstract.
summary: The goal of this project was to create a comprehensive and cartographically refined thematic map illustrating the annual precipitation patterns across China. This project showcases a complete GIS workflow, from raw data processing and advanced spatial analysis to final map production and design.

tags:
- Undergraduate Project
- Spatial Analysis
- ArcGIS

featured: false

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
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
#   focal_point: ""
#   preview_only: false

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

For this project, I undertook a complete GIS workflow to produce a high-quality thematic map of China's annual precipitation. The process began with extensive data preparation, where I sourced, cleaned, and processed vector data for national boundaries, rivers, and meteorological stations, establishing an Albers Equal Area projection for accuracy. A key part of this stage was building a custom, cartographically sound base map that correctly represented all of China's territories, including the South China Sea Islands via an inset map.

The core of the analysis involved transforming point data from weather stations into a continuous surface. I used the advanced geostatistical method of Co-kriging, leveraging elevation as a secondary variable to create a more accurate precipitation model. Finally, I focused on detailed cartographic design in ArcGIS, classifying the data with an intuitive color scheme, generating and labeling contour lines (isohyets), and assembling a polished final map layout with all essential elements. The resulting map effectively visualizes complex environmental data through clear and professional cartography.



<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
