---
title: "Automated MPI code generation for scalable finite-difference solvers"
authors:
- admin
date: "2024-03-27T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2024-03-27T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: Partial differential equations (PDEs) are crucial in modelling diverse phenomena across scientific disciplines, including seismic and medical imaging, computational fluid dynamics, image processing, and neural networks. Solving these PDEs on a large scale is an intricate and time-intensive process that demands careful tuning. This paper introduces automated code-generation techniques specifically tailored for distributed memory parallelism (DMP) to solve explicit finite-difference (FD) stencils at scale, a fundamental challenge in numerous scientific applications. These techniques are implemented and integrated into the Devito DSL and compiler framework, a well-established solution for automating the generation of FD solvers based on a high-level symbolic math input. Users benefit from modelling simulations at a high-level symbolic abstraction and effortlessly harnessing HPC-ready distributed-memory parallelism without altering their source code. This results in drastic reductions both in execution time and developer effort. While the contributions of this work are implemented and integrated within the Devito framework, the DMP concepts and the techniques applied are generally applicable to any FD solvers. A comprehensive performance evaluation of Devito's DMP via MPI demonstrates highly competitive weak and strong scaling on the Archer2 supercomputer, demonstrating the effectiveness of the proposed approach in meeting the demands of large-scale scientific simulations.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin # condimentum.

tags:
- Source Themes
featured: false

links:
- name: Custom Link
  url: http://example.org
url_pdf: https://arxiv.org/abs/2312.13094
# url_code: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_dataset: '#'
url_poster: 'https://www.devitoproject.org/presentations/devito-mpi-poster.pdf'
# url_project: ''
# url_slides: ''
# url_source: '#'
# url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ""
  preview_only: false

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

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
