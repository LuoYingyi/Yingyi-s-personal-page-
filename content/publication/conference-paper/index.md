---
title: "AlN Sputtering Parameter Estimation Using A Multichannel Parallel DCT Neural Network"

# Authors
# If you have author profile folders under content/authors/, use their folder names instead.
authors:
  - Yingyi Luo
  - Talha M. Khan
  - Emadeldeen Hamdan
  - Xin Zhu
  - Hongyi Pan
  - Didem Ozevin
  - A. Enis Çetin

# Author notes (optional)
author_notes: []

# Publication (paper) date – use the conference date so sorting works as expected.
date: '2024-04-22T00:00:00Z'
doi: '10.1109/VTS60656.2024.10538771'

# Schedule page publish date (NOT publication's date).
# You can set this to now if you want it to appear on the site immediately.
publishDate: '2024-04-22T00:00:00Z'

# Publication type (CSL)
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: '2024 IEEE 42nd VLSI Test Symposium (VTS)'
publication_short: 'IEEE VTS 2024'

# Abstract – paste the official abstract text here.
abstract: >
  In this paper, we present a method for estimating the deposition parameters of the thin film material Aluminum Nitride (AIN) using a deep neural network. The neural network predicts the AIN orientations, which are critical for micromachining Micro-Electro-Mechanical Systems (MEMS) transducers such as accelerometers and acoustic emission sensors. The network features three parallel channels, each equipped with a Discrete Cosine Transform (DCT) based layer that encodes the input parameters into a latent space. This DCT layer applies a hard-thresholding nonlinearity to eliminate noise from the input parameters, resulting in a sparse representation of the latent space. Trained with a dataset comprising AlN orientations parameters and their optimal values, our model is adept at simultaneously extracting and integrating various essential frequency components. Experimental results underscore the effectiveness of our proposed approach in achieving accurate and comprehensive estimation of AlN orientations and MEMS design parameters, thereby providing a promising path for advanced optimization.

# Summary. An optional shortened abstract.
summary: > 
  We propose a multichannel parallel DCT neural network to estimate key process
  parameters in AlN sputtering from in-situ signals, aiming at faster calibration
  and process control. 

tags:
  - AlN
  - Sputtering
  - Discrete Cosine Transform
  - Neural Networks
  - Process Parameter Estimation

# Display this page in the Featured widget?
featured: true

# Custom links (optional)
# - name: Preprint
#   url: https://...
links: []

# URLs (add what you have; leave empty strings if none)
url_pdf: ''            # e.g. 'uploads/AlN_DCTNN_VTS2024.pdf'
url_code: ''           # e.g. 'https://github.com/...'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: 'https://ieeexplore.ieee.org/document/10538771'
url_video: ''

# Featured image
# Put featured.jpg/png in this page folder to show a thumbnail on the list page.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
projects: []

# Slides (optional) – if you have a Markdown slide deck under content/slides/
slides: ''
---
