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

### 2. Traffic!

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

[Steps to create an Alarm on CloudWatch]

## AutoScaling and Load Balancing

Autoscaling automatically adjust the amount of computational resources based on traffic coming from the server.
An Auto Scaling group contains a collection of EC2 instances that are treated as a logical grouping for the purposes of automatic scaling and management. An Auto Scaling group also enables us to use Amazon EC2 Auto Scaling features such as health check replacements and scaling policies. Both maintaining the number of instances in an Auto Scaling group and automatic scaling are the core functionality of the Amazon EC2 Auto Scaling service.

_Load balancer_: It distributes traffic between EC2 instances, so that no instance is overwhelmed

<img width="643" alt="Screenshot 2022-08-24 at 16 22 40" src="https://user-images.githubusercontent.com/102330725/186457937-588c84b1-5e5f-458a-8781-79965d6f61e9.png">

## AutoScaling Steps

### Create a template

1. We start by launching a template, Go to Launch Templates ---> Create launch template

![Screenshot 2022-08-25 at 15 34 50](https://user-images.githubusercontent.com/102330725/186865060-af0f073d-bdab-4281-bfeb-0838d74ccd05.png)

2. Provide a name and description for the template and tick the checkbox for AutoScaling guidance.

![Screenshot 2022-08-25 at 11 39 15](https://user-images.githubusercontent.com/102330725/186869409-89cd810c-e0e7-4c11-9ea4-8fd7bcdd0186.png)

3. Select an Amazon Machine Image

![Screenshot 2022-08-26 at 10 12 06](https://user-images.githubusercontent.com/102330725/186870546-3f9ca791-9813-4dea-af13-d08fe040ee76.png)

4. Select **t2 micro** as an Instance Type

![Screenshot 2022-08-26 at 10 15 38](https://user-images.githubusercontent.com/102330725/186871173-9ce2853e-a6dc-4205-945a-ed50722e7d3f.png)

5. Add the key

![Screenshot 2022-08-26 at 10 27 43](https://user-images.githubusercontent.com/102330725/186873622-909eb4f5-5721-4494-8ca1-8faa666fca17.png)

6. Add security group

![Screenshot 2022-08-26 at 10 30 29](https://user-images.githubusercontent.com/102330725/186874235-395d22b4-12b1-4441-aaad-4826ea3c66ed.png)

7. Add storage

![Screenshot 2022-08-26 at 10 31 13](https://user-images.githubusercontent.com/102330725/186874462-431c1762-b08c-40c2-8dee-62d627e35eaa.png)

8. Add resource tags and Advanced details if needed and then click on Create template below the summary

![Screenshot 2022-08-26 at 10 33 42](https://user-images.githubusercontent.com/102330725/186875443-cad19188-a5d5-4697-b174-7b496fd2c9cf.png)

### AutoScaling

1. Go to Autoscaling groups --> Create an Autoscaling group

![Screenshot 2022-08-26 at 10 49 32](https://user-images.githubusercontent.com/102330725/186891032-bce78964-c3f4-439e-8c7a-4ad69dc04842.png)
