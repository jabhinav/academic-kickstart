---
title: Scanned PDF-to-HTML Conversion
summary: Extract structured information from unstructured documents.
tags:
- OCR Improvement
- Deep Learning
- Super Resolution
- Loss Formulation
date: "2017-08-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: Link
  url: https://github.com/jabhinav/Super-Resolving-Documents
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
In practice, scanned PDF documents are converted into consumable representations (HTML/JSON) to drive structured data extraction. However, poor quality document images suffer from low token fidelity when an OCR engine such as Tessearct is used for token extraction.  To remedy this, we leveraged deep learning based solutions for document quality enhancement and delivered the same for public release as part of IBM's Watson API. We formulated a novel `Text Quality Improvement Loss' for the standard super-resolution convolutional neural network (SRCNN) to generate high-resolution text images. The proposed framework identifies text regions from images and minimizes additional MSE between such localised regions on top of the standard MSE, enforced by Single Image Super Resolution frameworks. This results in simultaneous optimisation of perceptual quality of the image and the OCR performance.

Moreover, we provied (a) hybrid PDF support to extract data from documents containing both scanned and programmatic content, (b) capability to handle skewed documents, (c) multi-lingual support for data extraction from documents with over 50 different languages and (d) extraction service for detecting logos, bar-codes and signatures for downstream document processing such as querying, retrieval etc.
