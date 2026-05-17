# 🌐 Distributed Systems Basics

## Overview

A distributed system is a computing model where multiple independent machines work together as a single unified system.

These machines communicate over a network and coordinate to perform tasks at scale.

<br><br>

## Key Characteristics

- **Scalability** → ability to handle increasing workloads by adding nodes  
- **Fault Tolerance** → system continues operating even if some nodes fail  
- **Concurrency** → multiple processes run in parallel  
- **Transparency** → users perceive the system as a single unit  
- **Decentralization** → no single point of control or failure  

<br><br>

## Core Components

- **Nodes** → individual machines in the system  
- **Network** → communication layer between nodes  
- **Storage Systems** → distributed data storage (e.g., MinIO, HDFS)  
- **Coordination Services** → manage synchronization and consistency  
- **Processing Engines** → distributed computation (e.g., Spark)  

<br><br>

## Common Architectures

### Client–Server Model
A central server provides services to multiple clients.

### Peer-to-Peer (P2P)
All nodes are equal and share resources directly.

### Data Pipeline Architecture
Data flows through stages such as ingestion → processing → storage → analytics.

<br><br>

## Example in This Project

This project uses a distributed architecture:

- Data ingestion via scrapers  
- Storage in MinIO (Data Lake)  
- Processing with PySpark  
- NLP and sentiment analysis layer  
- FastAPI serving analytics  
- Dashboard visualization with Streamlit  

<br><br>

## Technologies Used

- Apache Spark (PySpark)  
- MinIO (S3-compatible storage)  
- FastAPI  
- Docker  
- Streamlit  
- Distributed file formats (Parquet, JSON)  

<br><br>

## Benefits in Big Data Systems

- high scalability for large datasets  
- efficient parallel processing  
- resilience to failures  
- modular architecture design  
- improved performance over single-machine systems  

<br><br>

## Summary

Distributed systems enable modern data platforms to process large-scale information efficiently by dividing workloads across multiple machines working in coordination.
