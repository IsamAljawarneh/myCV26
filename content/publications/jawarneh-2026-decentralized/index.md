---
title: Decentralized Stratified Sampling for Low-Latency Approximate Geospatial Data
  Stream Processing in Edge-Cloud Architectures
authors:
- Isam Mashhour Al Jawarneh
- Lorenzo Felletti
- Luca Foschini
- Paolo Bellavista
date: '2026-05-03'
publishDate: '2026-05-03T15:03:42.758855Z'
publication_types:
- article-journal
publication: '*arXiv preprint arXiv:2605.01922*'
abstract: The exponential growth of geospatial data streams flowing from IoT devices challenges conventional cloud-based analytics, which typically suffer from network bandwidth waste and latency, basically attributed to the data being managed completely by Cloud, such as centralized sampling. To address this gap, we propose EdgeApproxGeo, a novel edge-cloud architecture that performs spatial-stratified online sampling at network edge devices near data sources. Our system introduces a novel sampling method called EdgeSOS, which is a unique decentralized, geohash-based stratified sampling algorithm designed to operate independently at resource-constrained edge nodes without cross-node synchronization, coupled with spatial-aware data distribution and topic routing in Apache Kafka data stream ingestion, aiming at optimizing downstream data stream processing analytics. We evaluated our system on two real-world geo-referenced datasets, mobility and air quality, and EdgeApproxGeo achieves a significant speedup over cloud-only baselines while maintaining errors in check (e.g., MAPE < 10% error rate at 80% sampling rate). We further demonstrate that coarser geohash granularity (e.g., Geohash-5) can reduce error figures by 30% as compared to finer counterparts (i.e., Geohash-6), thus revealing a tunable accuracy-efficiency trade-off. Our standard-compliant prototype, built atop Apache Kafka and Apache Spark, further validates the utility of edge-deployed approximate query processing for real-time big geospatial data analytics.

tags:
- Parallel, and Cluster Computing

featured: true

hugoblox:
  ids:
    arxiv: 2605.01922v1

links:
- type: preprint
  provider: arxiv
  id: 2605.01922v1
- type: code
  url: "#"
- type: slides
  url: "#"
- type: dataset
  url: "#"
- type: poster
  url: "#"
- type: source
  url: "#"
- type: video
  url: "#"
- type: custom
  label: Custom Link
  url: "#"

---
