# How to Answer System Design Questions

> A step-by-step approach to structuring your response in system design interviews.

---

## 1. Clarify Requirements

- **Scale:** How many users? What is the expected growth?
- **Performance:** What are the latency or throughput requirements?
- **Core Features:** What are the must-have vs. nice-to-have features?

## 2. Estimate Scale

- Requests per minute (RPM)
- Data storage needs
- Bandwidth and traffic patterns
- Read vs. write ratio

## 3. High-Level Design

- Start with a simple architecture (e.g., web server + database)
- Gradually add complexity as needed (e.g., caching, load balancing, sharding)
- Identify and address bottlenecks

---

_Tip: Communicate your thought process clearly and iterate on your design as new requirements or constraints are discussed._
