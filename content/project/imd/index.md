---
title: 'The Correlation between IMD and Education Levels'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2024-05-19T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
# publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
# publication_types: ['paper-']

# Publication name and optional abbreviated publication name.
# publication: In *Hugo Blox Builder Conference*
# publication_short: In *ICW*

# abstract: The Index of Multiple Deprivation (IMD) provides a comprehensive measure of deprivation across different regions in the UK. While the specific methodologies vary slightly between countries, IMD generally accounts for factors such as income, employment, education, health, crime, housing access, and environmental quality. This project focuses on London, exploring the relationship between IMD and education levels to better understand how deprivation may impact educational attainment across the city.

# Summary. An optional shortened abstract.
summary: This project aimed to investigate the relationship between socioeconomic deprivation and educational attainment across London. The central question was - Is there a measurable link between living in a deprived area and having lower educational qualifications, and what does this pattern look like geographically?

# tags:
#   - Master Project
#   - Visualisation
#   - Python

# Display this page in the Featured widget?
featured: false


# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: 'https://github.com/LufeiYue1/GEOG5990_Assignment'
# url_dataset: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_video: 'https://youtube.com'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#   focal_point: ''
#   preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---
In this project, I investigated the link between socioeconomic deprivation and educational attainment in London. Using Python libraries like Pandas and GeoPandas, I integrated Index of Multiple Deprivation (IMD) data, census statistics on qualifications, and LSOA boundary shapefiles to create a comprehensive dataset for analysis. My goal was to quantify this relationship statistically and visualize it geographically.
My analysis followed a two-step process. An initial Spearman's rank correlation test across all education levels did not yield a statistically significant result. However, a deeper dive using a boxplot to compare deprivation with the percentage of residents having no qualifications revealed a clear trend: more deprived areas consistently have a higher proportion of people with no formal education. To visualize this spatially, I created a choropleth map, which showed a distinct concentration of high deprivation in inner and eastern London, contrasted with more affluent areas on the city's outskirts. This project highlights the importance of combining different analytical techniques to uncover nuanced patterns and provides a clear, data-driven map for understanding social inequality in London.

<!-- 
{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
