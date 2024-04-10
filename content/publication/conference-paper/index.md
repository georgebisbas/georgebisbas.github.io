---
title: 'Temporal blocking of finite-difference stencil operators with sparse “off-the-grid” sources'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Fabio Luporini
  - Mathias Louboutin
  - Rhodri Nelson
  - Gerard J. Gorman
  - Paul H.J. Kelly

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2021-08-28T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2021-08-28T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In 2021 IEEE International Parallel and Distributed Processing Symposium (IPDPS)
publication_short: In IPDPS'21 

abstract: Stencil kernels dominate a range of scientific applications, including seismic and medical imaging, image processing, and neural networks. Temporal blocking is a performance optimization that aims to reduce the required memory bandwidth of stencil computations by re-using data from the cache for multiple time steps. It has already been shown to be beneficial for this class of algorithms. However, applying temporal blocking to practical applications' stencils remains challenging. These computations often consist of sparsely located operators not aligned with the computational grid (“off-the-grid”). Our work is motivated by modelling problems in which source injections result in wavefields that must then be measured at receivers by interpolation from the grided wavefield. The resulting data dependencies make the adoption of temporal blocking much more challenging. We propose a methodology to inspect these data dependencies and reorder the computation, leading to performance gains in stencil codes where temporal blocking has not been applicable. We implement this novel scheme in the Devito domain-specific compiler toolchain. Devito implements a domain-specific language embedded in Python to generate optimized partial differential equation solvers using the finite-difference method from high-level symbolic problem definitions. We evaluate our scheme using isotropic acoustic, anisotropic acoustic, and isotropic elastic wave propagators of industrial significance. After auto-tuning, performance evaluation shows that this enables substantial performance improvement through temporal blocking over highly-optimized vectorized spatially-blocked code of up to 1.6x.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: [temporal blocking, stencils, dsl, hpc, ipdps]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
# url_code: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_dataset: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_poster: ''
# url_project: ''
url_slides: ''
# url_source: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_video: 'https://youtube.com'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
