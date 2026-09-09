---
title: Students Supervised
summary: Master's degree students I have supervised or co-supervised, along with their research outcomes and current positions.
date: 2018-06-28T00:00:00Z

reading_time: false  # Show estimated reading time?
share: false  # Show social sharing links?
profile: false  # Show author profile?
comments: false  # Show comments?

# Optional header image (relative to `assets/media/` folder).
header:
  caption: ""
  image: ""
---

{{< hl >}}I have co-advised several undergraduate researchers within the last five years.{{< /hl >}}

## An example outstanding undergraduate student's project that I co-supervised recently:

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

## Master's Degree Students Supervised

> [!NOTE]+ Lorenzo Felletti
> **Thesis:** *Decentralized Stratified Sampling for Low-Latency Approximate Geospatial Data Stream Processing in Edge-Cloud Architectures*
> 
> **Publication:** Co-authored journal article in *Cluster Computing* (Springer)
> {{< button url="https://link.springer.com/article/10.1007/s10586-026-06219-1" new_tab="true" style="primary" size="sm" icon="document-text" >}}Read Paper{{< /button >}}
> 
> **Current Position:** SysDev @ Amazon

{{< spoiler text="Click here to view thesis details" >}}
Lorenzo's thesis introduced **EdgeApproxGeo**, a novel edge-cloud architecture featuring:

-   **EdgeSOS Algorithm**: A decentralized, geohash-based stratified sampling method operating independently on resource-constrained edge nodes without cross-node synchronization
-   **Spatial-Aware Kafka Routing**: Neighborhood-based topic partitioning derived from geohash-to-polygon mapping, eliminating costly network shuffles during Spark aggregation
-   **Rust Implementation**: Parallel execution using `rayon` achieving near-linear scaling up to 100K tuples/batch with <100ms latency

Validated on Shenzhen electric taxi mobility & Chicago hyperlocal air quality datasets, demonstrating a **1.2× speedup** over cloud-only baselines while maintaining MAPE < 10% at 80% sampling fraction.
{{< /spoiler >}}

--------------------------------------------------------------------------------------------

> [!NOTE]+ Madyan Omar
> **Research Focus:** Multi-agent LLM frameworks with spatial knowledge graphs for context-aware urban planning and health analytics
> 
> **Publication:** Co-authored journal article in *Information Processing & Management* (Elsevier)
> {{< button url="https://www.sciencedirect.com/science/article/pii/S0306457326004760" new_tab="true" style="primary" size="sm" icon="document-text" >}}Read Paper{{< /button >}}
> 
> **Additional Output:** Several conference papers in related venues

{{< spoiler text="Click here to view research details" >}}
Madyan's research bridges the gap between plain Large Language Models and geospatial reasoning through structured knowledge grounding. Key contributions include:

-   **GeoAgent-MG-RAG Framework**: Multi-agent system integrating dynamic Geospatial Multi-modal Knowledge Graphs (GeoMMKG) with Retrieval-Augmented Generation
-   **Brain Orchestrator**: Achieves **97.5% tool-call accuracy** across four foundation models (Llama 4, GPT OSS, Kimi K2, Qwen3) using few-shot learning on 160 natural language queries
-   **Multi-Objective Optimization**: Successfully identifies Pareto-optimal solutions balancing distance, pollution exposure, and scenic value for route planning tasks
-   **POI Recommendation**: Maintains high positional relevance (NDCG > 0.6) even as query complexity increases

This work provides a scalable template for adapting multi-modal large language models to spatial public health challenges in smart city analytics.
{{< /spoiler >}}

--------------------------------------------------------------------------------------------

### Previous Supervision Experience

- At [University of Bologna](https://www.unibo.it), I had the honor to serve as a co-advisor for several undergraduate and graduate research projects (from 2017 through 2021) that are related to `NoSQL data warehousing` and `big data management`.
- Before 2016, At [University of Business and Technology](https://www.ubt.edu.sa/About/Home) (from 2013 to 2015), I supervised several undergraduate final year graduation projects in several CS areas.