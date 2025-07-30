```
- Are there dashboards to monitor --> Consistency, Availability, and Partition Tolerance. If not, what tools ?

No, there are no direct dashboards for Consistency, Availability, and Partition Tolerance.
However, tools like Prometheus, Grafana, CloudWatch, which help monitor


- Any tips to detect/mitigate/recover - load balancer failures in a distributed system ?

Detect load balancer failures using health checks, monitoring with tools like prom , grafana , etc.., and error rate alerts. Mitigate by deploying redundant LBs across zones/regions and using gloabal load balancers.


- As part of SLA, SLO, SLI - do we define circuit breaker ?

No, circuit breakers are not defined as part of SLA/SLO/SLI — they are resilience mechanisms at the system design level.
However, SLIs/SLOs may influence when to trigger a circuit breaker (e.g., if error rate exceeds an SLO threshold), but the circuit breaker itself is part of implementation, not the SLA contract.


```
