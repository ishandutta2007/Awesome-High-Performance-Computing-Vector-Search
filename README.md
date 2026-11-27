# Awesome-High-Performance-Computing-Vector-Search

# Awesome-High-Performance-Computing-Vector-Search



Top High Performance Computing Vector Search (Opensource) 🌟 Star if you like it! 🌟



A curated list of top high-performance computing (HPC) vector search engines, embedding databases, ANN (Approximate Nearest Neighbor) libraries, and hybrid retrieval platforms—featuring commercial SaaS/Hosted platforms alongside their open-source equivalents.



---



## Table of Contents



- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source Equivalents & Tools](#open-source-equivalents--tools)

  - [Distributed & Production Vector Databases](#distributed--production-vector-databases)

  - [Embedded, Edge & High-Performance Local Vector Engines](#embedded-edge--high-performance-local-vector-engines)

  - [Core ANN Libraries & GPU-Accelerated Kernels](#core-ann-libraries--gpu-accelerated-kernels)

  - [Database Extensions for Vector Search](#database-extensions-for-vector-search)

  - [Multimodal & Hybrid Search Engines](#multimodal--hybrid-search-engines)

- [Contributing](#contributing)



---



## SaaS/Hosted Platforms



Commercial, fully managed, and cloud-hosted vector database services and enterprise hybrid search platforms.



* **[Pinecone](https://pinecone.io)** - Proprietary, serverless cloud vector database engineered for low-latency, high-throughput similarity search at billion-vector scale.

* **[Qdrant Cloud](https://qdrant.io)** - Managed cloud service for the Qdrant vector database offering automated scaling, backups, and distributed clustering.

* **[Weaviate Cloud](https://weaviate.io)** - Fully managed SaaS platform for Weaviate providing hybrid vector + keyword search, multi-tenancy, and built-in vectorization modules.

* **[Zilliz Cloud (Milvus)](https://zilliz.com)** - Enterprise managed cloud service built by the creators of Milvus featuring GPU-accelerated indexing (CAGRA) and tiered storage.

* **[Chroma Cloud](https://trychroma.com)** - Hosted serverless offering of the AI-native Chroma embedding database for rapid RAG and LLM application deployment.

* **[Vespa Cloud](https://vespa.ai)** - Managed big data serving engine supporting real-time tensor computations, vector search, and lexical ranking at massive scale.

* **[Elastic Cloud](https://elastic.co)** - Managed Elasticsearch platform offering dense vector search, HNSW indexing, and hybrid BM25 + semantic retrieval.

* **[Marqo Cloud](https://marqo.ai)** - End-to-end managed tensor search platform combining inference and vector storage for multimodal text and image retrieval.

* **[Deep Lake (Activeloop)](https://activeloop.ai)** - Managed cloud database for AI built specifically for storing, querying, and streaming multimodal tensors and embeddings.

* **[DataStax Astra DB](https://datastax.com)** - Serverless, multi-cloud DBaaS built on Apache Cassandra with native JVector-powered high-performance vector search.



---



## Open-Source Equivalents & Tools



Free and open-source software (FOSS) vector databases, SIMD/GPU-accelerated ANN libraries, embedded search engines, and database extensions.



### Distributed & Production Vector Databases



* **[Qdrant](https://github.com)** - High-performance, open-source vector similarity search engine written in Rust featuring SIMD hardware acceleration, quantization, and rich payload filtering.

* **[Milvus](https://github.com)** - Cloud-native, distributed open-source vector database designed for billion-scale similarity search with disaggregated storage and compute.

* **[Weaviate](https://github.com)** - Open-source, AI-native vector database written in Go supporting HNSW indexing, hybrid BM25F + vector search, and GraphQL/REST APIs.

* **[Vald](https://github.com)** - Highly scalable, distributed open-source vector search engine built on the ultra-fast NGT algorithm and Kubernetes-native architecture.

* **[Vespa](https://github.com)** - Open-source, high-performance big data serving engine capable of low-latency ANN vector search, tensor evaluation, and machine-learned ranking.

* **[OpenSearch](https://github.com)** - Community-driven, open-source search and analytics suite supporting k-NN vector search backed by Faiss, NMSLIB, and Lucene.



### Embedded, Edge & High-Performance Local Vector Engines



* **[Needle (cactus-compute)](https://github.com)** - Ultra-fast, lightweight, and embedded vector search engine optimized for high-performance local and edge compute workloads.

* **[Chroma](https://github.com)** - Open-source AI-native embedding database designed for developer productivity with both in-memory/embedded and client-server modes.

* **[LanceDB](https://github.com)** - Open-source, serverless vector database built on the columnar Lance data format offering zero-copy disk-based ANN search in Rust and Python.

* **[sqlite-vec](https://github.com)** - Extremely small, zero-dependency, pure-C vector search SQLite extension capable of running anywhere from servers to edge devices.

* **[DuckDB VSS](https://github.com)** - Open-source extension bringing HNSW-accelerated vector similarity search directly into the high-performance DuckDB analytical engine.

* **[Orama](https://github.com)** - Fast, zero-dependency open-source full-text and vector search engine written in TypeScript for browsers, edge workers, and Node.js.



### Core ANN Libraries & GPU-Accelerated Kernels



* **[Faiss (Facebook AI Similarity Search)](https://github.com)** - Industry-standard C++/CUDA library by Meta for efficient similarity search and clustering of dense vectors on CPU and multi-GPU clusters.

* **[USearch](https://github.com)** - Smaller, faster single-file C++11/Rust/Python HNSW vector search engine leveraging hardware SIMD instructions (AVX-512, NEON) and user-defined metrics.

* **[DiskANN](https://github.com)** - Microsoft Research's graph-based ANN library (Vamana) engineered for billion-scale vector search directly from NVMe SSDs with minimal RAM.

* **[Hnswlib](https://github.com)** - Header-only C++ library implementing Hierarchical Navigable Small World (HNSW) graphs, serving as the core engine behind numerous vector databases.

* **[cuVS (NVIDIA RAPIDS)](https://github.com)** - Open-source GPU-accelerated vector search and clustering library featuring CAGRA, IVF-PQ, and brute-force CUDA primitives.

* **[ScaNN (Scalable Nearest Neighbors)](https://github.com)** - Google Research's open-source library for efficient vector similarity search at scale using anisotropic vector quantization.

* **[Voyager](https://github.com)** - Spotify's fast, low-memory open-source approximate nearest-neighbor search library written in C++ with Python and Java bindings.

* **[Annoy (Approximate Nearest Neighbors Oh Yeah)](https://github.com)** - Lightweight C++ library with Python bindings using random projection trees and memory-mapped files for shared-memory reads.



### Database Extensions for Vector Search



* **[pgvector](https://github.com)** - Open-source vector similarity search extension for PostgreSQL supporting exact and approximate nearest neighbor search (HNSW and IVFFlat).

* **[pgvecto.rs](https://github.com)** - High-performance Rust-based PostgreSQL vector extension supporting SIMD optimizations, binary quantization, and low-memory indexing.

* **[Pgai / pgvectorscale](https://github.com)** - Open-source PostgreSQL extension implementing DiskANN-inspired StreamingDiskANN indexes for high-performance, cost-efficient vector search.

* **[Redis Stack / RediSearch](https://github.com)** - High-throughput in-memory search engine module supporting real-time HNSW and FLAT vector indexing alongside secondary filtering.

* **[Apache Cassandra (JVector)](https://github.com)** - Pure-Java embedded vector search engine utilizing DiskANN-style graph algorithms and SIMD acceleration to power Cassandra 5.0.



### Multimodal & Hybrid Search Engines



* **[Marqo](https://github.com)** - Open-source tensor search engine integrating CLIP, OpenCLIP, and HuggingFace models directly into the indexing and query pipeline.

* **[Deep Lake](https://github.com)** - Open-source dataset and tensor storage format enabling version-controlled multimodal embeddings and rapid streaming to PyTorch/TensorFlow.

* **[Meilisearch](https://github.com)** - Lightning-fast, open-source Rust search engine supporting hybrid semantic vector + typo-tolerant lexical search.

* **[Typesense](https://github.com)** - Open-source, in-memory search engine written in C++ offering built-in vector search, auto-embeddings, and hybrid ranking.



---



## Contributing



Contributions are welcome! Feel free to open a Pull Request to add more open-source vector databases, HPC ANN kernels, or SIMD/GPU-accelerated search engines.



1. Fork the repository.

2. Add your project under the appropriate category with a concise description.

3. Submit a Pull Request.
