# Common System Design Patterns

> Key architectural patterns and best practices for scalable, reliable systems.

---

## 1. Microservices Architecture

- **Service Discovery:** Mechanisms for locating services in a distributed system
- **API Gateway:** Central entry point for client requests, routing, authentication, and rate limiting
- **Inter-Service Communication:** REST, gRPC, message queues, etc.
- **Data Partitioning:** Strategies like sharding and consistent hashing
- **CAP Theorem:** Understand trade-offs between Consistency, Availability, and Partition Tolerance; how it impacts database choice

## 2. Monitoring and Observability

- **Logging:** Centralized and structured logs for troubleshooting
- **Metrics:** Collect and analyze system and application metrics
- **Alerting:** Automated alerts for anomalies or failures
- **Data Encryption:** Secure data at rest and in transit

---

_Tip: Use these patterns as building blocks and adapt them to the specific requirements of your system._
