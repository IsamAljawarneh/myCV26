---
title: Students Supervised
summary: Master's degree students I have supervised or co-supervised, along with their research outcomes and current positions.
date: 2026-09-09T00:00:00Z

reading_time: false  # Show estimated reading time?
share: false  # Show social sharing links?
profile: false  # Show author profile?
comments: false  # Show comments?

# Optional header image (relative to `assets/media/` folder).
header:
  caption: ""
  image: ""
---



## Master's Degree Students Supervised

> [!NOTE]+ Lorenzo Felletti
> **Thesis:** *Edge Cloud Computing for Geospatial Data Processing and Approximate Queries*
> 
> **Publication:** Co-authored journal article in *Cluster Computing* (Springer)
> {{< button url="https://link.springer.com/article/10.1007/s10586-026-06219-1" new_tab="true" style="primary" size="sm" icon="document-text" >}}Read Paper{{< /button >}}
> 
> **Current Position:** SysDev @ Amazon

{{< spoiler text="Click here to view thesis details" >}}
**Thesis Title:** *Edge Cloud Computing for Geospatial Data Processing and Approximate Queries*

Lorenzo's thesis proposed a novel edge-cloud architecture designed to offload preprocessing workloads from cloud clusters by leveraging lightweight edge nodes positioned near IoT data sources. Key contributions include:

-   **Geohash-Based Stratified Sampling**: Edge nodes calculate geohashes for incoming tuples and perform decentralized stratified sampling locally, ensuring spatial representativeness without cross-node synchronization
-   **Spatial-Aware Data Distribution**: Sampled data is routed to neighborhood-specific Apache Kafka topics via geohash-to-polygon mapping, enabling efficient downstream aggregation in Apache Spark
-   **Containerized Pipeline Prototype**: The entire data pipeline—from IoT ingestion through edge preprocessing to cloud analytics—was deployed using Docker for portability and horizontal scaling

The system was prototyped using real-world taxi trajectory data from Shenzhen (17M+ population), demonstrating that edge-based geohash sampling and spatial-aware routing significantly reduce cloud computational load while preserving statistical accuracy for approximate geospatial queries.
{{< /spoiler >}}

--------------------------------------------------------------------------------------------

> [!NOTE]+ Madyan Omar
> **Research Focus:** TBA
> 
> **Publication:** Co-authored journal article in *Information Processing & Management* (Elsevier)
> {{< button url="https://www.sciencedirect.com/science/article/pii/S0306457326004760" new_tab="true" style="primary" size="sm" icon="document-text" >}}Read Paper{{< /button >}}
> 
> **Additional Output:** Several conference papers in related venues

{{< spoiler text="Click here to view research details" >}}
Madyan's research bridges the gap between plain Large Language Models and geospatial reasoning through structured knowledge grounding. Key contributions include:

TBD

This work provides a scalable template for adapting multi-modal large language models to spatial public health challenges in smart city analytics.
{{< /spoiler >}}

--------------------------------------------------------------------------------------------

{{< hl >}}I have co-advised several undergraduate researchers within the last five years.{{< /hl >}}

## An example 
outstanding undergraduate student's project that I co-supervised recently:

{{< hl >}}project title{{< /hl >}}: *QoS-aware Cloud-based Meteo and Mobility Data Processing at Scale*

{{< hl >}}student{{< /hl >}}: [Denis Pereira](https://ie.linkedin.com/in/denis-pereira/en) currently `DevOps Engineer` at [workday Ireland](https://www.workday.com/en-us/homepage.html)

{{< hl >}}My Role{{< /hl >}}:  **`Co-Advisor`** with Prof. [Paolo Bellavista](https://www.unibo.it/sitoweb/paolo.bellavista/en)

{{< hl >}}Year{{< /hl >}}:  `2021`

{{< hl >}}Code{{< /hl >}}:  [Code](https://github.com/denper1/MeteoMobilityIntegration)


{{< spoiler text="Click here to view the project description" >}}
**Project Description**
Our student worked on a novel algorithm that enables the seamless integration of georeferenced mobility and meteorological data streams. The purpose is to generate a unified view that enables joint analytics. Advanced queries are then supported, such as `what are the Top-5 polluted neighborhoods in NYC, where vehicle mobility rates are high`. The project aims at enabling insightful analytics that foster the culture of planning the cities in a way that reduces the impact of air-borne pollutants (such as PM10 and PM2.5) on the health of the lightweight dwellers.

{{< /spoiler >}}

--------------------------------------------------------------------------------------------

### Previous Supervision Experience

- At [University of Bologna](https://www.unibo.it), I had the honor to serve as a co-advisor for several undergraduate and graduate research projects (from 2017 through 2021) that are related to `NoSQL data warehousing` and `big data management`.
- Before 2016, At [University of Business and Technology](https://www.ubt.edu.sa/About/Home) (from 2013 to 2015), I supervised several undergraduate final year graduation projects in several CS areas.