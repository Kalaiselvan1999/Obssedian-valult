## NoSQL Databases: A Concise Overview

**NoSQL databases** are designed for flexible data models and scalable performance. They offer ease of development, functionality, and performance at scale.

**Key features and benefits:**

- **Flexible schemas:** NoSQL databases can accommodate different data structures, making them adaptable to evolving requirements.
- **Scalability:** They can handle large datasets and high traffic efficiently, ensuring performance in modern applications.
- **Ease of development:** NoSQL databases often have simpler development processes compared to traditional relational databases.

## NoSQL Databases: A Flexible Solution for Modern Applications

### Key Benefits of NoSQL Databases

- **Flexibility:** NoSQL databases offer flexible schemas, making them suitable for semi-structured and unstructured data. This enables faster and more iterative development.
- **Scalability:** NoSQL databases are designed to scale horizontally by adding more nodes to a cluster, rather than vertically by increasing the capacity of individual servers. This provides better scalability and cost-effectiveness.
- **High Performance:** NoSQL databases are optimized for specific data models and access patterns, leading to improved performance compared to relational databases.
- **Functionality:** NoSQL databases offer rich APIs and data types tailored to their respective data models, providing a wide range of functionalities.
## Summary: NoSQL Database Use Cases

**Real-time data management:**

- Deliver real-time recommendations, personalization, and improved user experiences.
- Example: Disney+ uses Amazon DynamoDB to scale and deliver features like Continue Watching, Watchlist, and Personalized Recommendations.

**Cloud security:**

- Use graph databases to discover complex relationships within data.
- Example: Wiz uses Amazon Neptune to identify and fix critical security risks by uncovering toxic combinations of risk factors.

**High-availability applications:**

- Build high-availability, low-latency applications for messaging, social media, file sharing, and more.
- Example: Snapchat uses NoSQL database systems to reduce message sending latency by 20%.
## How NoSQL Databases Work

### Key Characteristics of NoSQL Databases

- **Flexible Data Models:** NoSQL databases use various data models, often JSON, to accommodate diverse data structures.
- **Large Data Volumes:** Optimized for handling massive amounts of data.
- **Low Latency:** Designed for quick data access, reducing response times.
- **Relaxed Consistency:** Trade-offs in data consistency for improved performance and scalability.

### How NoSQL Databases Function

- **Data Models:** Use flexible data models like JSON to represent data as name-value pairs.
- **Optimized for Performance:** Prioritize speed and scalability over strict data consistency.
- **Diverse Implementations:** Varying approaches based on the specific data model.
## NoSQL vs. Relational Databases: A Book Database Example

### Relational Databases

- **Normalization:** Data is split into multiple tables to reduce redundancy.
- **Relationships:** Primary and foreign keys define connections between tables.
- **Structure:** Optimized for storage and referential integrity.

### NoSQL Databases

- **Documents:** Each book is stored as a single document.
- **Attributes:** All relevant data (ISBN, title, author, etc.) is within the document.
- **Structure:** Optimized for development and scalability.
![[Pasted image 20240905221731.png]]

## Types of NoSQL Databases

### Key-Value Databases

- Store data as a collection of key-value pairs.
- Highly partitionable and scalable.
- Suitable for gaming, ad tech, and IoT.
- Example: Amazon DynamoDB.

### Document Databases

- Store data as JSON objects.
- Flexible, semi-structured, and hierarchical.
- Suitable for catalogs, user profiles, and content management systems.
- Examples: Amazon DocumentDB (with MongoDB compatibility), MongoDB.

### Graph Databases

- Store data as nodes and edges.
- Suitable for highly connected datasets.
- Use cases include social networking, recommendation engines, fraud detection, and knowledge graphs.
- Example: Amazon Neptune.

### In-Memory Databases

- Store data in memory for microsecond response times.
- Suitable for gaming, ad tech, and real-time analytics.
- Examples: Amazon MemoryDB for Redis, Amazon ElastiCache, Amazon DynamoDB Accelerator (DAX).

### Search Databases

- Dedicated to searching data content.
- Use indexes to categorize similar characteristics.
- Suitable for unstructured data like images and videos.
- Example: Amazon OpenSearch Service.
## Relational vs. NoSQL Databases

**Key Differences**

|Feature|Relational Databases|NoSQL Databases|
|---|---|---|
|**Data Model**|Tabular (rows and columns)|Key-value, document, graph, column|
|**Schema**|Strictly defined|Flexible, schema-less or dynamic|
|**ACID Properties**|Strong adherence|Trade-offs for performance and scalability|
|**Performance**|Dependent on disk subsystem|Dependent on hardware cluster, network latency, and application|
|**Scale**|Typically scale up or out|Typically scale out horizontally|
|**APIs**|Structured Query Language (SQL)|Object-based APIs|
|**Optimal Workloads**|Transactional, strongly consistent OLTP, OLAP|Low-latency applications, analytics over semi-structured data|

**In Summary**

Relational databases are well-suited for transactional and analytical workloads, while NoSQL databases offer flexibility and scalability for a variety of data access patterns. The choice between the two depends on the specific requirements of the application, such as data consistency, performance, and scalability.

## When to Choose NoSQL Databases Over SQL Databases

### Key Advantages of NoSQL Databases

- **Flexible Schemas:** Ideal for rapidly evolving data structures and iterative development.
- **Performance Prioritization:** Suitable for applications where speed is more important than strong data consistency and relationships.
- **Horizontal Scaling:** Supports scaling by distributing data across multiple servers.
- **Semi-structured and Unstructured Data:** Accommodates data that doesn't fit neatly into predefined tables.

### Hybrid Approach: Combining SQL and NoSQL

- **Leverage the Best of Both Worlds:** Use SQL for structured data and NoSQL for flexible, unstructured data.
- **Optimize Performance and Cost:** Match each workload to the most appropriate database for optimal results.

# NoSQL Databases

1. [[MongoDB]]
2. [[Cassandra]]
3. [[Scylla]]
4. [[Redis Cloud]]

