# DATA IN THE CLOUD — EXAM NOTES

## 1. Relational Databases in the Cloud
Relational databases store data in tables (rows + columns).  
In the cloud, these databases run on cloud servers instead of local machines.

Examples:
- Amazon RDS  
- Google Cloud SQL  
- Azure SQL  

### Benefits:
- Automatic backups  
- High availability  
- Easy scaling  
- No hardware required  
- Pay-as-you-go model  
- Accessible from anywhere  

---

## 2. Cloud File Systems: GFS and HDFS

### 2.1 GFS (Google File System)
- Designed by Google for large-scale data processing.
- Master–slave architecture.
- Stores very large files (GB–TB).
- High fault tolerance (data replicated on multiple machines).
- Provides high throughput.
- Used internally for Google Search, Maps, YouTube.

### 2.2 HDFS (Hadoop Distributed File System)
- Inspired by GFS.
- Part of Hadoop ecosystem.
- Stores data across many low-cost machines.
- Fault-tolerant using data replication.
- Suitable for batch jobs and big data analytics.
- Provides high data throughput.

---

## 3. BigTable, HBase, and Dynamo

### 3.1 BigTable (Google)
- Google’s NoSQL, column-family database.
- Highly scalable and distributed.
- Used in Gmail, Google Maps, YouTube.
- Designed for massive structured data.

### 3.2 HBase (Apache)
- Open-source equivalent of BigTable.
- Runs on top of HDFS.
- Supports real-time read/write access.
- Good for sparse and large datasets.

### 3.3 Dynamo (Amazon)
- Amazon’s distributed key-value NoSQL store.
- Decentralized (peer-to-peer).
- Highly available (no single point of failure).
- Used in Amazon's e-commerce systems.

---

## 4. MapReduce and Extensions

### 4.1 Parallel Computing
- Breaking a large task into smaller tasks.
- Running those tasks simultaneously on multiple machines.
- Results in faster processing and efficiency.

### 4.2 The MapReduce Model
MapReduce has two main phases:

#### 1. Map Phase:
- Input data is split into chunks.
- Map function processes each chunk.
- Produces intermediate key-value pairs.

#### 2. Reduce Phase:
- Key-value pairs are grouped by key.
- Reduce function aggregates values.
- Final output is generated.

### Advantages:
- Easy programming model.
- Automatic parallelization.
- Fault tolerance.
- Scales to thousands of machines.

---

# 5. MICEF Computing (Mist, IoT, Cloud, Edge, Fog)

## 5.1 IoT (Internet of Things)
- Network of physical devices with sensors.
- Devices collect and exchange data.
- Examples: smartwatches, smart lights, ACs, CCTV.

## 5.2 Cloud Computing
- Centralized data storage and processing.
- Remote servers (AWS, GCP, Azure).
- High scalability but higher latency.
- Requires internet connection.

## 5.3 Edge Computing
- Processing happens near the user/device.
- Low latency and real-time response.
- Reduces cloud load.
- Examples: routers, local hubs, phones.

## 5.4 Fog Computing
- Middleware layer between Edge and Cloud.
- Fog nodes perform intermediate processing.
- Reduces network congestion.
- Used in smart city and IoT systems.

## 5.5 Mist Computing
- Ultra-light computing inside IoT devices.
- Data processed directly on sensors.
- Extremely low latency.
- No dependence on cloud.

---

# 6. Applications of MICEF Computing
- Smart homes  
- Smart cities  
- Industrial IoT  
- Autonomous vehicles  
- Healthcare monitoring  
- Real-time analytics  

---

# SUMMARY TABLE

| Concept | Meaning |
|--------|---------|
| GFS | Google file system for big data |
| HDFS | Hadoop file system |
| BigTable | Google NoSQL database |
| HBase | Open-source BigTable |
| Dynamo | Amazon key-value NoSQL store |
| MapReduce | Parallel data processing model |
| IoT | Internet-connected smart devices |
| Edge | Processing near device |
| Fog | Layer between edge & cloud |
| Mist | Processing inside sensor |
| Cloud | Centralized servers |
