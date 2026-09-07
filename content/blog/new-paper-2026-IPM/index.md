---
title: 🌍 GeoAgent-MG-RAG: Multi-Agent LLM Framework with Spatial Knowledge Graphs
summary: Announcing our new paper on context-aware urban planning and health analytics using multi-agent LLMs integrated with dynamic spatial knowledge graphs.
date: 2026-09-07
authors:
  - me
tags:
  - GeoAI
  - Large Language Models
  - Spatial Knowledge Graphs
  - Urban Planning
  - Health Analytics
  - Retrieval-Augmented Generation
cover:
  image: cover.jpg
  icon:
    name: "🗺️"
image:
  caption: "GeoAgent-MG-RAG Architecture Overview"
  focal_point: Center
  placement: 1
content_meta:
  trending: true
---

We are thrilled to announce the acceptance of our new paper **"GeoAgent-MG-RAG: A multi-agent LLM framework with spatial knowledge graphs for context-aware urban planning and health analytics"**! 🎉

{{< toc mobile_only=true is_open=true >}}

## Why This Matters

> [!TIP]
> **Bridging the Gap**: Plain Large Language Models struggle with geospatial reasoning and hallucinations. Our framework addresses these limitations by integrating multi-agent systems with dynamic spatial knowledge graphs for evidence-based urban intelligence.

Current Geographic AI (GeoAI) systems face critical challenges:
- **Hallucination problems** in spatial reasoning
- **Fragmented single-task engines** that cannot unify heterogeneous data
- **Lack of real-time decision-making** capabilities for complex urban workflows
- **Rigid query-response patterns** instead of autonomous agent workflows

Our solution transforms how we approach smart city analytics by combining the power of multi-agent orchestration with structured geospatial knowledge retrieval.

## Key Innovations

### 🧠 Multi-Agent Architecture
GeoAgent-MG-RAG introduces a three-layer architecture:
1. **Perception Layer**: Ingests multi-modal urban data streams (air quality sensors, satellite imagery, POIs, elevation models)
2. **Brain Orchestrator**: Performs intent classification, query decomposition, and manages spatial context through location-based subgraph retrieval
3. **Action Layer**: Executes domain-specific workflows via tool-calling APIs interfaced with context-aware spatial embeddings

### 📊 Spatial RAG Paradigm
Unlike traditional semantic knowledge graph approaches, our **Geospatial RAG** retrieves spatially-aggregated subgraphs that embed multi-modal contextual attributes including:
- Air quality metrics (PM2.5 levels)
- Environmental indices (NDVI for vegetation)
- Scenic density features
- Real-time sensor readings

This enables real-time, evidence-based spatial reasoning with minimal hallucination.

## Performance Highlights

Our comprehensive evaluation demonstrates exceptional results:

| Metric | Achievement |
|--------|-------------|
| **Tool-Call Accuracy** | 97.5% (peak performance across 4 foundation models) |
| **Models Tested** | Llama 4, GPT OSS, Kimi K2, Qwen3 |
| **Test Queries** | 160 natural language queries |
| **POI Recommendation** | NDCG > 0.6 (high positional relevance) |
| **Multi-Objective Optimization** | Successfully identifies Pareto-optimal solutions |

### Supported Workflows

The framework currently supports four main spatial geo-processing workflows:

1. **Multi-objective context-aware route planning** - Balancing distance, pollution exposure, and scenic value
2. **Personalized air pollution exposure assessment** - Through spatiotemporal aggregation
3. **Urban scenario simulation** - PM2.5 prediction using NHITS model for green infrastructure planning
4. **Context-aware POI recommendation** - Considering order of intent and maintaining high positional relevance

## Dataset & Evaluation

We validated our framework on comprehensive multi-modal datasets from **Chicago and NYC**, including:
- Thousands of graph nodes and Points of Interest (POIs)
- Raster data files (NDVI, DEM)
- OpenStreetMap networks
- AlphaEarth embeddings from geospatial Foundation Models
- Hyperlocal air quality sensor data

## How to Use

### For Researchers

1. **Access the code**: The implementation will be available on our GitHub repository
2. **Run the demos**: We provide Jupyter notebooks demonstrating each workflow
3. **Extend the framework**: The modular design allows easy integration of new data sources and workflows

## Impact on Smart Cities

> [!IMPORTANT]
> **Real-World Applications**: Our framework enables actionable insights for public health monitoring, sustainable urban planning, and human mobility optimization.

This work addresses the critical "urban intelligence gap" by transforming massive multi-modal geospatial data streams into unified decision support systems. Unlike previous approaches that focus solely on question-answering or single-task predictions, GeoAgent-MG-RAG provides a general-purpose spatial reasoning engine capable of orchestrating diverse urban analytics workflows.

## Comparison with Existing Approaches

| Feature | CityGPT | GeoLLM | GeoGraphRAG | **GeoAgent-MG-RAG** |
|---------|---------|--------|-------------|---------------------|
| Multi-agent orchestration |  | ❌ | ❌ | ✅ |
| Dynamic spatial KG | ❌ | ❌ | Partial | ✅ |
| Real-time decision making | ❌ | ❌ | ❌ | ✅ |
| Multi-objective optimization | ❌ | ❌ | ❌ | ✅ |
| Tool-call accuracy | N/A | N/A | ~85% | **97.5%** |

## Next Steps

- **Read the full paper**: Available on arXiv (link coming soon)
- **Try the demos**: Explore our Jupyter notebooks showcasing the four core workflows
- **Join the community**: Contribute to the open-source implementation
- **Cite this work**: If you use GeoAgent-MG-RAG in your research, please cite our paper

## Acknowledgments

This research was supported by advances in geospatial foundation models, multi-agent systems, and knowledge graph technologies. We thank the broader GeoAI and information science communities for inspiring this work.

---

**Keywords**: Geospatial artificial intelligence (GeoAI); Large Language Models (LLMs); Spatiotemporal analytics; Agent-based AI; Spatial knowledge graphs; Retrieval-Augmented Generation (RAG)

Happy researching! 🚀🌍