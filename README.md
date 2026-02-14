# Advanced Data Management Project

This repository contains the final project for the **Advanced Data Management** course (MSc in Computer Science, 2025/2026).

## 📌 Project Overview

The project models and analyzes a football domain dataset using a query-driven design approach.  
A complete workload of 10 analytical and operational queries was defined and used as the basis for data modeling and system comparison.

The project includes:

- Conceptual modeling (ER diagram)
- Logical design for multiple NoSQL systems
- Partition key and super-identifier analysis
- Index design and efficiency evaluation
- Implementation and query validation

## ⚙️ Systems Evaluated

The same workload was implemented and analyzed in:

- **MongoDB**
- **Cassandra**
- **Neo4j**

For each system, we evaluated:

- Query admissibility
- Aggregation support
- Partitioning strategy
- Indexing mechanisms
- Suitability for analytical workloads

## 🧠 Design Strategy

The workload consists mainly of aggregation-heavy queries such as:

- Total minutes played by players (seasonal and global)
- Top-K players by total minutes
- Stadium attendance statistics
- Filtering valuation data by date ranges
- Multi-entity retrieval queries

Based on workload analysis and system capabilities, **MongoDB was identified as the most suitable system**, due to:

- Native aggregation framework
- Aggregate-oriented modeling
- Efficient handling of nested documents
- Reduced query complexity through controlled denormalization

Cassandra was limited due to lack of aggregation support over nested collections.  
Neo4j, while suitable for relationship traversal, was less aligned with the analytical nature of the workload.

## 📊 Dataset

A real-world football dataset (few MB) was transformed into JSON and imported into MongoDB (`football_db`), following the aggregate-oriented schema defined in the logical design.

## 📄 Repository Contents

- `ADM-Project.pdf` — Full project report including:
  - Workload definition
  - ER modeling
  - Logical schema design
  - MongoDB implementation
  - Cassandra evaluation
  - Neo4j graph modeling
  - System comparison and final conclusions

## 🎯 Academic Context

University of Genoa  
Master’s in Computer Science  
Course: Advanced Data Management  
Academic Year: 2025/2026
