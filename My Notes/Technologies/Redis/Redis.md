
---
### **Redis Use Cases & Internals**

Redis is an **in-memory, key-value store** with use cases in caching, real-time analytics, and session management.

#### **Common Use Cases**

- **Caching:** Store frequently accessed data to **reduce DB queries** (e.g., API responses).
- **Session Management:** Store user sessions with TTL (**Time-to-Live**) for **fast retrieval**.
- **Pub/Sub Messaging:** Used for **real-time communication** (e.g., chat applications).
- **Rate Limiting:** Control API requests using **increment counters** (e.g., per second, per user).

#### **How Redis Works Internally?**

- Uses **DS like Hashes, Lists, Sets, Sorted Sets** for efficient storage.
- **Single-threaded** but highly optimized using **event loops**.
- **Data Persistence:**
    - **RDB (Redis Database Backup):** Takes snapshots at intervals.
    - **AOF (Append-Only File):** Logs every operation for durability.
- Uses **LRU (Least Recently Used)** eviction policy for memory optimization.