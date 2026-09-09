---
title: "⚡️ EdgeApproxGeo: Low-Latency Geospatial Stream Processing at the Edge"
summary: Announcing our new journal article on decentralized stratified sampling for real-time IoT analytics in edge-cloud architectures.
date: 2026-09-09
authors:
  - me
tags:
  - Edge Computing
  - Geospatial Analytics
  - Approximate Query Processing
  - Apache Kafka
  - Apache Spark
  - IoT
image:
  caption: "EdgeApproxGeo Architecture Overview"
  focal_point: Center
cover:
  image: featured.jpg
  position:
    x: 50
    y: 40
  overlay:
    enabled: true
    type: "gradient"
    opacity: 0.3
    gradient: "bottom"
  fade:
    enabled: true
    height: "80px"
  icon:
    name: "🌐"
content_meta:
  trending: true
---

We are excited to announce the acceptance of our new journal article **"Decentralized Stratified Sampling for Low-Latency Approximate Geospatial Data Stream Processing in Edge-Cloud Architectures"**! 🎉

{{< toc mobile_only=true is_open=true >}}

## Why This Matters

> [!TIP]
> **Bridging the Edge-Cloud Gap**: Traditional cloud-based geospatial analytics suffer from bandwidth waste and latency. Our system moves intelligent sampling to the network edge, reducing data transfer while preserving statistical accuracy.

Processing petabyte-scale geospatial data streams from IoT devices (e.g., vehicle telematics, air quality sensors) presents a critical challenge: **exact query processing is too slow and expensive**. While Approximate Query Processing (AQP) offers a solution, existing systems either ignore spatial characteristics or force all raw data to the cloud before sampling.

Our work introduces **EdgeApproxGeo**, a novel architecture that performs statistically rigorous, geohash-based stratified sampling *directly on resource-constrained edge nodes*.

## Key Innovations

### 🧠 EdgeSOS Algorithm
We introduce **EdgeSOS** (Edge-based Spatial-aware Online Sampling), a unique decentralized algorithm that:
- Operates independently on each edge node without cross-node synchronization
- Uses geohash-based stratification to preserve spatial representativeness
- Is implemented in **Rust** with parallel execution (`rayon`) for near-linear scaling
- Maintains <100ms latency even for batches of 100K tuples

### 📊 Spatial-Aware Data Routing
Unlike standard pub/sub brokers, our system extends **Apache Kafka** with:
- Neighborhood-based topic partitioning derived from geohash-to-polygon mapping
- O(1) neighborhood lookups via precomputed inverted hashmaps
- Elimination of costly network shuffles during downstream Spark aggregation

## Performance Highlights

Our evaluation on real-world datasets (Shenzhen electric taxi mobility & Chicago hyperlocal air quality) demonstrates:

| Metric | Achievement |
|--------|-------------|
| **Speedup vs Cloud-Only** | 1.2× average (15–20% reduction in execution time) |
| **Accuracy at 80% Sampling** | MAPE < 10% (virtually indistinguishable from ground truth) |
| **Geohash Granularity Trade-off** | Geohash-5 reduces error by ~30% vs Geohash-6 |
| **Scalability** | Near-linear scaling up to 100K tuples/batch |
| **Throughput** | Stable ~20K messages/batch at ~100ms latency |

### Tunable Accuracy-Efficiency Trade-offs

> [!NOTE]
> Coarser geohash granularities improve statistical stability. At 80% sampling fraction, Geohash-5 achieves ~7% MAPE compared to ~10% for Geohash-6—a 30% relative improvement—while maintaining actionable spatial resolution for smart city analytics.

## Real-World Validation

We validated our system on two diverse real-world datasets:

- **Shenzhen Electric Taxi Dataset**: ~1.16M GPS trajectories from 664 vehicles, testing high-speed urban mobility analytics
- **Chicago Air Quality Dataset** (Project Eclipse): ~130K hyperlocal PM2.5 sensor readings, testing environmental monitoring scalability on Microsoft Azure HDInsight

Both deployments confirm that edge-based preprocessing significantly reduces end-to-end latency without sacrificing the statistical utility required for operational decision-making.

## Comparison with Existing Approaches

| Feature | SAOS/SpatialSSJP | AgileDART | GeoEkuiper | **EdgeApproxGeo** |
|---------|------------------|-----------|------------|-------------------|
| Deployment | Cloud-only | Edge | Edge/Cloud | **Edge/Cloud** |
| Spatial Strata | ✅ | ❌ | ❌ | ✅ |
| Decentralized Sampling | ❌ | ❌ |  | ✅ |
| AQP Support | ✅ | ❌ | ❌ | ✅ |
| Spatial-Aware Routing | ❌ | ❌ | ❌ | ✅ |
| Error Bounds | ✅ | ❌ | ❌ | ✅ |

## Next Steps

- **Read the full paper**: Available on arXiv ([arXiv:2605.01922v1](https://arxiv.org/abs/2605.01922))
- **Try the prototype**: Clone the repository and deploy the Docker containers
- **Cite this work**: If you use EdgeApproxGeo in your research, please cite our article
- **Future work**: We plan to support H3/S2 tessellations, sliding windows, and serverless edge deployment

## Acknowledgments

This work has been partially supported by the European Union under the NRRP partnership on "Telecommunications of the Future" (PE00000001 - program "RESTART") and by the National PRIN JOULE project.

---

**Keywords**: edge computing; approximate query processing; geospatial sampling; Apache Kafka; Apache Spark; stratified sampling

Happy researching! 🚀