# Monitoring and Alert Management

![Screenshot 2022-08-24 at 14 20 06](https://user-images.githubusercontent.com/102330725/186428948-2d7e0aa5-547b-43fc-aa1d-9b3660dff26d.png)

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

![Screenshot 2022-08-24 at 14 21 00](https://user-images.githubusercontent.com/102330725/186429139-0a525837-11f3-44b3-82cd-3692af5fc731.png)


## What is Alert Management?

An Alert Management System (AMS) is a real time system which maintains profiles about threats, or other entities and in real time processes events and returns alerts and their risks.

### Actions taken in case of an alert

- Manually remediate the alert.
- Acknowledge an alert that requires attention.
- Create an incident or security incident.
- Create a case.
- Close the alert.
- Resolve any incident that is related to the alert.
- Reopen the alert

## SNS And SQS?

SQS and SNS in AWS — Simple Notification Service and Simple Queue Service.

SQS and SNS are important components for scalable, large scale, distributed, cloud-based applications:

SNS is a distributed publish-subscribe service. Messages are pushed to subscribers as and when they are sent by publishers to SNS.

SQS is distributed queuing service. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can be stored in SQS for short duration of time (max 14 days).

![Screenshot 2022-08-24 at 14 21 42](https://user-images.githubusercontent.com/102330725/186429313-37421268-ecc7-46a3-a9de-8f8b12452863.png)
