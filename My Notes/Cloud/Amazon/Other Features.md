
---
### **Amazon EC2 (Elastic Compute Cloud)**

- EC2 provides **resizable compute capacity** in the cloud, allowing us to run applications on virtual machines.
- We use EC2 instances to **deploy and host our backend services** with auto-scaling and load balancing to handle varying traffic.
- It supports different instance types optimized for compute, memory, and storage, based on our workload needs.

### **AWS Lambda**

- Lambda is a **serverless compute service** that runs code in response to events without managing servers.
- We use Lambda for **processing background tasks, event-driven workflows, and lightweight APIs**.
- It automatically scales based on request volume, making it cost-efficient for intermittent workloads.

### **AWS IAM (Identity and Access Management)**

- IAM helps in **managing user access and permissions** securely within AWS.
- We use IAM to **control who can access AWS resources** by defining roles, users, and policies.
- It supports **fine-grained access control** using policies to restrict actions based on roles and permissions.
- We also use **IAM roles for services like EC2 and Lambda** to grant them specific access without exposing credentials.
