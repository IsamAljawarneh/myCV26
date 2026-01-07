---
title: 'Line Simplification for Efficient Approximate Join Queries On Big Geospatial Data'

# Authors
authors:
  - Fatima Ahmed Alhammadi
  - Haya Almadhloum Alsuwaidi
  - Shooq Abdelrahman Alzarooni
  - me

date: '2024-01-01T00:00:00Z'

# Schedule page publish date (NOT publication's date).
publishDate: '2024-01-01T00:00:00Z'

# Publication type.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *2024 Fifth International Conference on Intelligent Data Science Technologies and Applications (IDSTA)*
publication_short: In *IDSTA '24*

abstract: Line simplification algorithms are widely used to reduce geometric complexity in vector-based geospatial datasets while preserving essential spatial characteristics. In this work, we investigate the integration of two prominent line simplification techniques—Douglas-Peucker (DP) and Visvalingam-Whyatt (VW)—into a filter-and-refinement framework for efficient spatial joins between large-scale georeferenced mobility and air quality datasets. We evaluate implementations using both the Shapely library and the Mapshaper web service, demonstrating that simplification can reduce polygon vertex counts by up to 94% while maintaining high analytical fidelity. Our experiments on New York City neighborhood polygons show that both DP and VW, when applied via Mapshaper, yield low approximation errors (MAPE ≈ 0.048–0.049), strong Spearman correlations (>0.88), and minimal Jensen-Shannon divergence, enabling faster spatial joins without compromising downstream tasks like clustering or regression.

summary: This paper demonstrates how line simplification (Douglas-Peucker and Visvalingam-Whyatt) drastically reduces geospatial polygon complexity—by 94%—enabling efficient spatial joins for big mobility and air quality data while preserving analytical accuracy.

tags:
  - Geospatial Data Science
  - Approximate Query Processing
  - Line Simplification
  - Spatial Join
  - Douglas-Peucker
  - Visvalingam-Whyatt
  - Big Data Management

# Display this page in the Featured widget?
featured: true

# Standard identifiers for auto-linking
hugoblox:
  ids:
    doi: 10.1109/IDSTA62194.2024.10747008

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
  caption: 'Simplified NYC neighborhood polygons after line simplification (from paper)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
projects:
  - line-simplification-geo

# Slides (optional).
slides: ""
---

> [!NOTE]
> Click the _Cite_ button above to import publication metadata into your reference management software.

This work addresses the computational bottleneck of spatial joins between massive point-based mobility data and high-resolution polygonal administrative boundaries (e.g., city neighborhoods). By applying line simplification as a preprocessing step, the authors significantly reduce the geometric complexity of polygons—enabling faster spatial containment checks during joins. Two algorithms (Douglas-Peucker and Visvalingam-Whyatt) are evaluated across two platforms (Shapely in Python and Mapshaper.org), with results showing that Mapshaper-based simplification achieves the best balance of topology preservation, minimal boundary overlap, and computational efficiency. The approach supports scalable geospatial analytics in smart cities, particularly for tasks requiring repeated spatial joins under strict QoS constraints.