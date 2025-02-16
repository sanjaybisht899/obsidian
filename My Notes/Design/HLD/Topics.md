### Complete System Design Tutorial Notes

---

### **Core Concepts of System Design**

1. **High-Level Architecture of a Computer**
   - Computers function through a layered system, each optimized for specific tasks.
   - **Bits and Bytes**: 
     - 1 bit = 0 or 1.
     - 1 byte = 8 bits (represents a single character or number).
     - Data storage units: KB, MB, GB, TB.
   - **Disk Storage**:
     - HDD or SSD.
     - Non-volatile (data persists without power).
     - SSDs are faster (500 MB/s to 3,500 MB/s) compared to HDDs (80 MB/s to 160 MB/s).
   - **RAM (Random Access Memory)**:
     - Volatile memory (requires power to retain data).
     - Holds active data (variables, applications, runtime stack).
     - Faster than SSDs (over 5,000 MB/s).
   - **Cache**:
     - Smaller than RAM (measured in MB).
     - Faster access times (few nanoseconds for L1 cache).
     - Stores frequently used data to optimize CPU performance.
   - **CPU**:
     - Fetches, decodes, and executes instructions.
     - Processes high-level code compiled into machine code.
   - **Motherboard**:
     - Connects all components and allows data flow.

---

### **High-Level Architecture of a Production-Ready App**

2. **CI/CD Pipeline**:
   - Automates code deployment from repository to production.
   - Tools: Jenkins, GitHub Actions.
3. **Load Balancers and Reverse Proxies**:
   - Distribute user requests across multiple servers.
   - Tools: NGINX.
4. **External Storage**:
   - Data stored on separate servers connected over a network.
5. **Logging and Monitoring**:
   - Tracks system interactions and stores logs externally.
   - Tools: PM2 (backend), Sentry (frontend).
6. **Alerting Services**:
   - Notifies developers of issues via platforms like Slack.
7. **Debugging**:
   - Identify issues using logs.
   - Replicate issues in a staging environment.
   - Use tools to debug and roll out hot fixes.

---

### **Pillars of System Design**

8. **Key Principles**:
   - **Scalability**: System grows with user base.
   - **Maintainability**: Future developers can understand and improve the system.
   - **Efficiency**: Optimal use of resources.
   - **Resilience**: System performs well even during failures.

9. **Core Elements**:
   - **Moving Data**: Optimize for speed and security.
   - **Storing Data**: Choose between SQL/NoSQL, understand access patterns, indexing, and backups.
   - **Transforming Data**: Convert raw data into meaningful information.

10. **CAP Theorem**:
   - **Consistency**: All nodes have the same data at the same time.
   - **Availability**: System is always operational.
   - **Partition Tolerance**: System works even during network disruptions.
   - A system can only achieve two out of three properties.

---

### **System Availability and Reliability**

11. **Availability**:
   - Measured in percentage (e.g., 99.9% availability = 8.76 hours downtime/year).
   - **Service Level Objectives (SLOs)**: Performance goals (e.g., response time < 300 ms).
   - **Service Level Agreements (SLAs)**: Formal commitments to users (e.g., 99.99% availability).

12. **Resilience**:
   - Implement redundant systems.
   - Design for graceful degradation.

13. **Performance Metrics**:
   - **Throughput**: Requests per second (RPS), queries per second (QPS), bytes per second.
   - **Latency**: Time to handle a single request.

---

### **Networking Basics**

14. **IP Addresses**:
   - IPv4: 32-bit (4 billion unique addresses).
   - IPv6: 128-bit (larger address space).
15. **Data Packets**:
   - Contain IP headers (sender/receiver IP addresses).
   - Governed by Internet Protocol (IP).
16. **Transport Layer**:
   - **TCP**: Reliable, ensures complete data delivery (e.g., HTTP).
   - **UDP**: Faster, less reliable (e.g., video calls).
17. **DNS (Domain Name System)**:
   - Translates domain names to IP addresses.
   - Types of records: A (IPv4), AAAA (IPv6).
18. **Networking Infrastructure**:
   - Public/private IP addresses.
   - Firewalls monitor and control traffic.
   - Ports identify specific services (e.g., 80 for HTTP, 22 for SSH).

---

### **Application Layer Protocols**

19. **HTTP**:
   - Request-response protocol (GET, POST, PUT, DELETE).
   - Status codes: 200 (success), 300 (redirection), 400 (client error), 500 (server error).
20. **WebSockets**:
   - Two-way communication for real-time updates (e.g., chat apps).
21. **Email Protocols**:
   - SMTP (sending), IMAP/POP3 (retrieving).
22. **File Transfer**:
   - FTP (file transfer), SSH (secure shell).
23. **Real-Time Communication**:
   - WebRTC (browser-to-browser communication), MQTT (IoT devices).

---

### **API Design**

24. **CRUD Operations**:
   - Create (POST), Read (GET), Update (PUT/PATCH), Delete (DELETE).
25. **API Paradigms**:
   - **REST**: Stateless, uses HTTP methods, JSON for data exchange.
   - **GraphQL**: Avoids over-fetching, uses POST for all requests.
   - **gRPC**: Built on HTTP/2, uses protocol buffers.
26. **Best Practices**:
   - Backward compatibility (versioning).
   - Rate limiting to prevent abuse.
   - CORS settings for cross-origin resource sharing.

---

### **Caching and CDNs**

27. **Caching**:
   - **Browser Caching**: Stores resources locally (HTML, CSS, JS).
   - **Server Caching**: Stores frequently accessed data (e.g., Redis).
   - **Database Caching**: Caches query results.
   - **Eviction Policies**: LRU, FIFO, LFU.
28. **CDNs (Content Delivery Networks)**:
   - Distribute static content (images, videos) from geographically close servers.
   - Types: Pull-based (automatic updates), Push-based (manual updates).

---

### **Proxy Servers**

29. **Types**:
   - **Forward Proxy**: Hides client IP, controls internet access.
   - **Reverse Proxy**: Hides server IP, used for load balancing, caching.
   - **Open Proxy**: Allows anonymous browsing.
   - **Transparent Proxy**: Visible to clients, used for caching.
30. **Use Cases**:
   - Instagram proxies for managing multiple accounts.
   - Internet use control and monitoring.
   - SSL offloading and web application firewalls.

---

### **Load Balancing**

31. **Algorithms**:
   - Round Robin, Least Connections, Least Response Time, IP Hashing, Consistent Hashing.
32. **Types**:
   - Hardware (F5 Big IP), Software (HAProxy, NGINX), Cloud-based (AWS ELB).
33. **Failover Strategies**:
   - Redundant load balancers, health checks, auto-scaling.

---

### **Databases**

34. **Types**:
   - **Relational (SQL)**: Tables, ACID compliance (e.g., PostgreSQL, MySQL).
   - **NoSQL**: Flexible, schema-less (e.g., MongoDB, Cassandra).
   - **In-Memory**: Fast, used for caching (e.g., Redis).
35. **Scaling**:
   - **Vertical Scaling**: Increase server resources (CPU, RAM).
   - **Horizontal Scaling**: Add more servers (sharding, replication).
36. **Performance Techniques**:
   - Caching, indexing, query optimization.

---
