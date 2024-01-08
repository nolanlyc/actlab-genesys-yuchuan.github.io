---
layout: about
title: about
permalink: /
subtitle: <a href='#'>Affiliations</a>. Address. Contacts. Moto. Etc.

profile:
  align: right
  image: genesys-logo.jpg
  image_circular: false # crops the image to make it circular
  more_info:

news: false  # includes a list of news items
latest_posts: false  # includes a list of the newest posts
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

_GeneSys_ is a programmable deep learning acceleration system generator.
The core computation engines in _GeneSys_ are a systolic array (for operations such as convolution) and SIMD engine (for operations such as ReLU and pooling). _GeneSys_ is parametrizable, and it is possible to automatically generate hardware with different numbers of processing elements, on-chip buffer configurations, and memory bandwidths.
The generated accelerator acts like a co-processor connected to the host via the PCIe bus.
The target workloads for the accelerator are computer vision and transformers-based models.
