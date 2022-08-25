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

Alerting gives timely awareness to problems in our cloud applications so we can resolve the problems quickly.

In Cloud Monitoring, an alerting policy describes the circumstances under which we want to be alerted and how we want to be notified.

When we use the console, we can enable a recommended alert or we can create an alert by starting from the Alerts page of Cloud Monitoring.

## SNS And SQS?

SQS and SNS in AWS — Simple Notification Service and Simple Queue Service.

SQS and SNS are important components for scalable, large scale, distributed, cloud-based applications:

SNS is a distributed publish-subscribe service. Messages are pushed to subscribers as and when they are sent by publishers to SNS.

SQS is distributed queuing service. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can be stored in SQS for short duration of time (max 14 days).

![Screenshot 2022-08-24 at 14 21 42](https://user-images.githubusercontent.com/102330725/186429313-37421268-ecc7-46a3-a9de-8f8b12452863.png)

## AutoScaling and Load Balancing

An Auto Scaling group contains a collection of EC2 instances that are treated as a logical grouping for the purposes of automatic scaling and management. An Auto Scaling group also enables us to use Amazon EC2 Auto Scaling features such as health check replacements and scaling policies. Both maintaining the number of instances in an Auto Scaling group and automatic scaling are the core functionality of the Amazon EC2 Auto Scaling service.

<img width="643" alt="Screenshot 2022-08-24 at 16 22 40" src="https://user-images.githubusercontent.com/102330725/186457937-588c84b1-5e5f-458a-8781-79965d6f61e9.png">

