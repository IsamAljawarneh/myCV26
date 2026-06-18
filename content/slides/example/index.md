---
title: "Efficiently Integrating Mobility and Environment Data for Climate Change Analytics"
date: 2021-10-25
# `type: slides` is inferred from folder, but can be set explicitly:
type: slides
slides:
  theme: black
  highlight_style: dracula
  diagram: true  # Enable Mermaid diagrams
  reveal_options:
    controls: true
    progress: true
    slideNumber: true
    hash: true
---

# Efficiently Integrating Mobility and Environment Data for Climate Change Analytics

### Isam Mashhour Al Jawarneh, Paolo Bellavista, Antonio Corradi, Luca Foschini, Rebecca Montanari
**Department of Computer Science and Engineering (DISI)**  
University of Bologna, Italy

*IEEE CAMAD 2021 | 25-27 October 2021, Virtual Conference*

---

## Outline

- **Background & Motivating Scenario**
  - Integrating mobility and meteorological data
  - Challenges & Requirements
- **MeteoMobil System**
  - Architectural design
  - Supported queries
- **Deployment & Evaluation**
  - Baselines and Testing setup
  - Results and Discussion
- **Conclusion & Future Work**

---

## Motivating Scenario

<div class="r-hstack">

<div style="flex: 1; padding-right: 1rem;">

### The Goal
- Study correlation between **vehicle pollutant emissions** and **health of dwellers** in metropolitan cities.
- Requires joining geo-referenced **mobility** and **meteorological** data (Spatial Join).
- Enables regular analytics of relationships between mobility patterns and climate change.

</div>

<div style="flex: 1; padding-left: 1rem;">

### The Impact
- **Interactive heatmap visualization**.
- Helps municipalities and city officials make strategic decisions for citizen health benefits.

![](https://images.unsplash.com/photo-1496568813637-05c3f8e58f0d?w=400&auto=format&fit=crop&q=60)
*Urban environment monitoring*

</div>

</div>

Note:
The core motivation is public health. By combining where people move (mobility) with what they breathe (meteorology/pollution), cities can make data-driven decisions.

---

## Requirements & Challenges

- **Shared Analytics**: Need to perform joint analysis on mobility and meteorological data.
- **Spatial Join**: Essential but computationally expensive.
- **Data Parametrization**:
  - Spatial data is parametrized (longitudes and latitudes).
  - Objects lose geometrical information during transformation.
  - Bringing parametrized tuples back into real geometries is expensive.

> **Key Challenge**: How to perform efficient spatial joins at scale?

---

## Solution: Efficient Spatial Join

### Filter-Refine Approach

1. **Generate Geocode**: Create codes for each tuple using Minimum Bounding Rectangles (MBRs).
2. **Generate MBRs**: Cover the space with MBRs.
3. **Filtering Step**: Apply a cheap MBR-join.
4. **Refinement Step**: Apply a costly join algorithm only on the remaining candidates to discard false positives.

Note:
This heuristic avoids checking every single pair of points by first filtering out obvious non-matches using coarse bounding boxes.

---

## MeteoMobil Architecture

```mermaid
graph LR
    A[Data Collector] -->|Georeferenced Data| B(Geospatial Encoder)
    B -->|Encoded Codes| C[Spatial Join Processor]
    D[Mobility Data] --> C
    E[Meteorological Data] --> C
    C -->|Unified Data| F[Query Processor]
    F --> G[Interactive Queries]
    
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style C fill:#bbf,stroke:#333,stroke-width:4px
    style F fill:#bfb,stroke:#333,stroke-width:2px