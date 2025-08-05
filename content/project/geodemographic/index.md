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

tags:
- Master Project
- K-means clustering
- ArcGIS Pro
- SPSS

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
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
#   focal_point: ""
#   preview_only: false

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
This project aimed to solve a real-world problem for the Leeds-based charity, Learning Partnerships. They needed to pinpoint neighbourhoods with the highest concentration of young, disadvantaged adults to effectively deploy a new support initiative. My goal was to transform raw census data into an actionable, location-based strategy for them. 

My approach involved creating a bespoke geodemographic classification. I began by strategically selecting key census variables that act as proxies for disadvantage, such as unemployment and low educational attainment. Using SPSS, I applied the K-means clustering algorithm to segment all of Leeds' neighbourhoods into four statistically distinct groups. The final step was to join this classification data to a map in ArcGIS Pro, allowing for a clear geographic visualization of the results.
![预印本封面](1.png)
![预印本封面](CLuster.png)
The analysis successfully identified a key target group, which I named the "Multilingual Multicultural Unemployment" cluster. As the final map revealed, these neighbourhoods are heavily concentrated in inner-city Leeds and are characterized by extremely high unemployment and significant language barriers. This output provides Learning Partnerships with an evidence-based strategy to focus their resources, tailor their services, and ultimately maximize their social impact by reaching the communities that need them most.
![预印本封面](featured.jpg)


<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
