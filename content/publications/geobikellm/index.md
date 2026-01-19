---
title: 'GeoBikeLLM: LLM-Powered Bike Route Planning with Air Quality and Vegetation-Aware Geospatial Intelligence'

# Authors
authors:
  - Sara Alshamsi
  - Menatalla Haggag
  - Lubana Al Rayes
  - Esraa Alhamid
  - Mohammad Alsmirat
  - Isam Al Jawarneh

date: '2025-01-01T00:00:00Z'

# Schedule page publish date (NOT publication's date).
publishDate: '2025-01-01T00:00:00Z'

# Publication type.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *2025 Sixth International Conference on Intelligent Data Science Technologies and Applications (IDSTA)*
publication_short: In *IDSTA '25*

abstract: Bike riding is widely embraced as a healthy, eco-friendly mode of transportation; thus, routes with cleaner air and greener surroundings are often preferred by cyclists seeking both physical well-being and enjoyable travel experiences. However, existing navigation systems rarely consider environmental conditions such as air pollution or vegetation density. To address this, we introduce **GeoBikeLLM**, a system that leverages Large Language Models (LLMs) for environment-aware bike route planning. Focused on Chicago, Illinois, USA, the system enables users to enter natural language prompts and their routing preferences—such as shortest, healthiest (low PM2.5), greenest (high NDVI), or a combination of these. The system integrates air quality, vegetation, and bicycle infrastructure datasets, applies KD-Tree-based spatial matching, and computes optimized paths using a weighted graph and Yen’s K-Shortest Paths algorithm. Data visualizations highlight spatial patterns in pollution and greenery. Evaluation using 35 user-generated prompts showed 94.3% accuracy in extracting both location entities and route preferences. GeoBikeLLM demonstrates how LLMs can enhance personalized, environmentally informed mobility experiences, offering a scalable solution for sustainable urban navigation.

summary: GeoBikeLLM is an LLM-powered system for environmentally aware bike route planning that integrates real-world air quality (PM2.5) and vegetation (NDVI) data to recommend routes prioritizing health and green exposure.

tags:
  - Geospatial AI
  - Large Language Models
  - Smart Cities
  - Environmental Mobility
  - Urban Sustainability
  - NDVI
  - Air Quality

# Display this page in the Featured widget?
featured: true

# Standard identifiers for auto-linking
hugoblox:
  ids:
    doi: 10.1109/IDSTA66210.2025.11202783

# Custom links
links:
  - type: pdf
    url: ""
  - type: code
    url: ""
  - type: dataset
    url: ""
  - type: slides
    url: ""
  - type: source
    url: ""
  - type: video
    url: ""

# Featured image
image:
  caption: 'Visualization of PM2.5 and NDVI spatial patterns in Chicago (from paper)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
projects:
  - geobikellm

# Slides (optional).
slides: ""
---

> [!NOTE]
> Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.

GeoBikeLLM represents a novel intersection of geospatial intelligence, environmental health, and natural language interfaces. By allowing cyclists to express routing preferences in everyday language—such as “Find me the cleanest-air route from Navy Pier to Hyde Park”—the system interprets intent via LLaMA 3.1, computes environmentally optimized paths using real PM2.5 and NDVI data, and explains results using LLaMA 3.3—all within a user-friendly Gradio interface. This work advances human-centered GeoAI and offers a blueprint for sustainable, health-aware urban mobility in smart cities.