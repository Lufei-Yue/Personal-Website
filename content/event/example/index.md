---
title: "High-Fidelity 3D Model Reconstruction using Air-Ground Fusion"
authors:
- admin
date: "2021-05-17T00:00:00Z"
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

# abstract: Standard 3D models created from UAV (drone) imagery are excellent for capturing large areas quickly, but they often suffer from significant limitations at ground level. Textures on building facades can be blurry, and complex structures like covered walkways or overhangs are often distorted or incomplete. This project aimed to solve this common industry problem by developing a method to enhance model accuracy and detail.

# Summary. An optional shortened abstract.
summary: Standard 3D models created from UAV (drone) imagery are excellent for capturing large areas quickly, but they often suffer from significant limitations at ground level. Textures on building facades can be blurry, and complex structures like covered walkways or overhangs are often distorted or incomplete. This project aimed to solve this common industry problem by developing a method to enhance model accuracy and detail.

tags:
- Undergraduate Project
- 3D models
- UAV

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
This project addressed a common challenge in 3D modeling where models generated solely from UAV (drone) data lack sufficient ground-level detail and texture clarity. My goal was to develop a cost-effective method to fuse aerial imagery with high-resolution, ground-based smartphone images to produce a single, high-fidelity 3D model of the Tianjin Normal University Library.

My methodology centered on unifying the two disparate datasets within a single coordinate system. I first created a detailed local model from the smartphone images, then used common tie points to perform an absolute orientation and similarity transformation on the UAV dataset. This precisely aligned the large-scale aerial model with the detailed ground model. By merging the two aligned datasets in ContextCapture, I was able to generate a final, integrated model.

The results were a significant success. The fused model exhibited crisp, clear textures and complete, accurate geometry for complex ground-level features like walkways and building entrances—details that were previously distorted or blurry. This project demonstrates a practical and scalable workflow for creating more realistic and accurate digital twins for urban planning and architectural visualization without relying on expensive, specialized equipment.

Drone modeling results:
![UAV](UAV.png)




<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
