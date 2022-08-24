# Monitoring and Alert Management

## What is Monitoring?

Monitoring is the process of collecting, aggregating, and analyzing metrics and displaying real-time quantitative data about a system to improve awareness of your components’ characteristics and behavior.
The data from various parts of our environment are collected into a monitoring system that is responsible for storage, aggregation, visualization, and initiating automated responses when the values meet specific requirements.

### Why is monitoring important

- Notification of when there is or could be a server issue and Alerting
- Providing a clear overview of all systems
- Fuel smarter decision making with historical data
- Ensuring better server performance over time

## The Four Golden Signals

### 1. Latency

It is important to distinguish between the latency of successful requests and the latency of failed requests.

### 2. Traffic

A measure of how much demand is being placed on your system, measured in a high-level system-specific metric.

### 3. Errors

The rate of requests that fail, either explicitly (e.g., HTTP 500s), implicitly (for example, an HTTP 200 success response, but coupled with the wrong content), or by policy.

### 4. Saturation

A measure of our system fraction, emphasizing the resources that are most constrained (e.g., in a memory-constrained system, show memory; in an I/O-constrained system, show I/O).

## What is CloudWatch?

- CloudWatch is a monitoring and management service that provides data and actionable insights for AWS, hybrid, and on-premises applications and infrastructure resources.
- We can collect and access all your performance and operational data in the form of logs and metrics from a single platform rather than monitoring them in silos (server, network, or database).
- CloudWatch enables us to monitor your complete stack (applications, infrastructure, and services) and use alarms, logs, and events data to take automated actions and reduce mean time to resolution (MTTR).
