# Backend Engineer aka Data Engineer

## Role

At our company, backend engineers architect, implement, and deploy distributed systems end-to-end to index and search blockchain data at massive scale.

Depending on your interests, this might mean building real-time data ingestion pipelines that process millions of transactions per second, designing search indexes that deliver sub-millisecond query responses, or obsessively optimizing distributed systems for global scale. Perhaps it involves solving infrastructure problems not yet conceived of in blockchain data processing.

## What You'll Build

You'll design systems that ingest data from dozens of blockchain networks in real-time, build distributed search indexes that handle billions of transactions, and create APIs that serve millions of queries with sub-second latency. You'll work directly with blockchain protocols, distributed databases, and high-performance computing.

Core technologies: Go/Rust, PostgreSQL, ClickHouse, Elasticsearch, Kafka, Docker, Kubernetes, AWS/GCP.

## Requirements

- 4+ years building distributed systems at scale
- Expert-level proficiency in Go or Rust
- Deep experience with databases and search technologies
- Understanding of distributed computing and system design
- Experience with high-throughput data processing

Bonus: blockchain infrastructure experience, time-series databases, real-time streaming systems.

## Task

### Pick one

1. load block metadata into PostgreSQL; build an API & a page to display  
   - ethereum-etl or BlockSci for extraction  
   - Postgres / Supabase free tier for storage  
   - PostgREST or Hasura CE for instant REST/GraphQL  
   - pg_trgm full-text module for optional block search

2. load NFT metadata into PostgreSQL; build an API & a page to display  
   - ethereum-etl-nft extension or Alchemy NFT API (free)  
   - Supabase / PostgREST / Hasura stack for API  
   - Fuse.js or pg_trgm for optional NFT search

3. build a Go Kafka consumer that streams mempool transactions into ClickHouse and exposes a low-latency API  
   - Sarama or confluent-kafka-go for Kafka client  
   - Redpanda Community (Kafka-compatible broker) for local dev  
   - clickhouse-go driver  
   - chi or gin for lightweight HTTP API  
   - Web3 `pendingTransactions` subscription via go-ethereum / Infura / Alchemy (free WS tier) for mempool source  
   - Blocknative Mempool API (free developer tier) as alternative data feed

4. backfill historical ERC-20 transfer events into Elasticsearch  
   - ethereum-etl for log extraction  
   - Elastic OSS / OpenSearch cluster  
   - Logstash or Beats for ingestion  
   - Kibana / OpenSearch Dashboards for quick validation

5. create a Rust microservice that computes and caches 24-hour token price aggregates in Redis and serves an OHLC endpoint  
   - axum or warp framework  
   - redis-rs crate for cache access  
   - tokio-cron-scheduler for periodic jobs  
   - coingecko or crypto-price crates for free market data

### Evaluation
- Quantitative (50%)
  - Data correctness & query accuracy: 25 pts
  - Throughput/latency benchmarks or resource usage: 10 pts
  - Automated tests & observability (metrics, logging): 15 pts
- Qualitative (35%)
  - Code structure & documentation: 15 pts
  - Scalability & reliability considerations explained: 10 pts
  - Communication of design decisions during interview: 10 pts
- AI Tool Use (15%)
  - Appropriate use of AI for boilerplate generation: 5 pts
  - Clear citation of AI-generated code in commits/comments: 5 pts
  - Ability to validate and correct AI output: 5 pts