---
title: Deep Metric Learning
summary: Video Representation Learning for Fine-Grained Scene Recognition and Retrieval.
tags:
- Deep Learning
- Event Recognition
- Loss Formulation
date: "2018-01-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: Link
  url: https://github.com/jabhinav/Deep-Video-Understanding
url_code: ""
url_pdf: "https://github.com/jabhinav/Deep-Metric-Learning-for-Video-Understanding/blob/master/Radial_Loss_Preprint.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
Advertising in digital media often requires recognition of critical scenes in videos for smart placement of brand advertisements. These critical scenes raise viewer anxiety and are a part of some parent activity. We distinguish them from the rest of non-critical scenes using an order-preserving fine-grained similarity metric that learns the required representations. The learned metric is tested in two novel tasks: video critical scene recognition and fine-grained video retrieval. To learn the metric, we proposed Pentuplet Loss and recently, an improved and more robust Radial Loss. 

These losses exploit the concept of `Quadlet Sampling' to mine data where each training sample is a tuple of query, positive, intermediate and negative samples. Finally, to ascertain the effectiveness of the loss in learning a deep metric for measuring similarities, we tested its performance against state-of-the-art baselines in the known tasks of fine-grained image retrieval and shot-boundary detection.
