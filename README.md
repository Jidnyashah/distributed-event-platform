# distributed-event-platform is a production-style, event-driven microservices system built using Spring Boot, Apache Kafka, PostgreSQL, Docker, and Kubernetes.

The goal of this project is to demonstrate how modern distributed systems process data asynchronously using event streaming, instead of tightly coupled service-to-service communication.

What Problem Does It Solve?

In traditional systems:

Services directly call each other (REST-to-REST)

Failures cascade

Scaling is difficult

Systems become tightly coupled

This project solves that by using:

Event-driven communication through Kafka

Services publish events instead of calling each other directly.

How It Works (Simple Flow)

Client sends a request to Order Service

Order Service stores data in PostgreSQL

Order Service publishes an event to Kafka

Other services (e.g., Notification Service, Analytics Service) consume the event

Each service processes independently

Tech Stack

Java 17

Spring Boot

Apache Kafka

PostgreSQL

Docker

Kubernetes

GitLab CI (or GitHub Actions)

Azure Kubernetes Service (optional deployment)
