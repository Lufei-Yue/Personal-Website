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

# abstract: In this project, I investigated the causal impact of London's Low Traffic Neighbourhoods (LTNs) on road safety. Analyzing a decade of city-wide accident data, I used Python to employ an advanced Difference-in-Differences (DID) model to move beyond simple correlation. The analysis revealed a statistically significant and lasting 10% annual reduction in traffic crashes in areas with LTNs. These findings provide robust causal evidence that LTNs are an effective long-term strategy for improving urban safety, offering a critical data point for policymakers shaping future transport initiatives. 

# Summary. An optional shortened abstract.
summary: Standard 3D models created from UAV (drone) imagery are excellent for capturing large areas quickly, but they often suffer from significant limitations at ground level. Textures on building facades can be blurry, and complex structures like covered walkways or overhangs are often distorted or incomplete. This project aimed to solve this common industry problem by developing a method to enhance model accuracy and detail.

# tags:
# - Undergraduate Thesis
# - 3D models
# - UAV

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

**🛠 Skills & Tools:** <kbd>ContextCapture</kbd> <kbd>Photogrammetry</kbd> <kbd>UAV/Drone Surveying</kbd> <kbd>3D Modelling</kbd> <kbd>Data Fusion</kbd>

---

## The Ground-Level Gap

In the field of 3D urban modelling, drones are exceptional at capturing roof structures and large-scale topography. However, they have one major limitation: the 'blind angle'. 

Models generated solely from aerial data often exhibit significant distortion at street level. Facades appear distorted and intricate details such as walkways and entrances lack texture clarity. My goal was to bridge this gap by developing a cost-effective workflow that fuses aerial imagery with high-resolution ground-based smartphone data to create a true digital twin.

My goal was to produce a single, high-fidelity 3D model with crisp ground-level details, without relying on expensive, specialised LiDAR equipment.

---

## Methodology: Multi-Source Data Fusion

My methodology focused on combining two different datasets — the "macro" view from the drone and the "micro" view from the smartphone — into a single coordinate system.

1.  **Data acquisition**: I captured an overview of the library using a drone, whilst simultaneously capturing ground-level details (façades, stairs and pillars) using a standard smartphone camera.
2.  **Local reconstruction**: I first processed the smartphone images to create a highly detailed local model.
3.  **Coordinate unification**: This was the crucial technical step. I used common tie points to perform absolute orientation and similarity transformation. This precisely aligned the large-scale aerial model with the detailed ground coordinates.
4.  **Integrated fusion**: Finally, I merged the aligned datasets in ContextCapture, creating a seamless mesh that retained the best features of both sources.

---

## Results: Visual Comparison

The difference in quality is immediately apparent. The picture below illustrates the difference in geometry and texture quality between the traditional UAV-only approach and my fused workflow.

| **Before: UAV Data Only** | **After: Multi-Source Fusion** |
| :---: | :---: |
| ![UAV Model Result](UAV.png) | ![Final Fused Result](after.png) |
| *Note the distorted geometry at the entrance and the blurry textures on the ground.* | *Clear textures and accurate geometry for complex features like stairs and pillars.* |

---

## Impact & Conclusion

The project successfully demonstrated that high-fidelity 3D modelling does not require a prohibitively large budget.

* **Holistic accuracy**: the fused model exhibits complete geometry for complex ground-level features that were previously distorted.<br>
* **Scalable workflow**: By demonstrating that smartphone data can be successfully integrated with aerial surveys, the project provides a practical solution for urban planning and architectural visualisation.
* **Cost-effectiveness**: It significantly reduces the barrier to creating realistic digital twins, bypassing the need for expensive ground-based laser scanners.



<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
