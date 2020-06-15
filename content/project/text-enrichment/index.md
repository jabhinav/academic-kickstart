---
title: Text Enrichment
summary: Enrichment of educational texts with supplementary information.
tags:
- Deep Learning
- AI for Education
- Information Extraction
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
  url: https://github.com/jabhinav/EducationEnrichment
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
Formal texts such as journal articles are composed of complex terminologies intended to be understood by targeted demographic. In absence of domain knowledge, they tend to be more ambiguous for general readers. To avail a complete semantic understanding of such texts for the readers, we proposed an enrichment system that mitigates the problem of searching for required information through heaps of sources. The system augments given text with required concept definitions, applications and concept dependency graphs. 

Our framework extracts key-concepts (technical terms) based on user discretion via a sequence of filtering stages - Linguistic Filtering, BBC Pruning and StackExchange Pruning. It detects the presence of required information by classifying each associated sentence into definition/application of the key-concept using a CNN-LSTM network. The same framework also runs on a data source such as Wikipedia to return the concept's missing definition and real-life application.
