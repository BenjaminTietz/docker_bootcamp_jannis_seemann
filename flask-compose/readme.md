# Flask, Redis and Nginx – Docker Compose Setup

This project demonstrates a simple multi-container application using Docker Compose.  
It consists of a Flask web application, a Redis cache, and an Nginx reverse proxy.

The focus of this project is not the application logic itself, but the interaction between services and the practical use of Docker Compose to wire them together.

---

## Services Overview

The stack is composed of three services:

### Redis (`db`)

- Uses the official `redis` image
- Acts as an in-memory cache or data store
- Exposed only inside the Docker network
- Not accessible from outside the Compose setup

### Flask Application (`webapp`)

- Custom-built Flask application
- Communicates with Redis for caching or shared state
- Exposes port 5000 internally for Nginx
- Designed to be scalable (multiple replicas when used with Swarm or `--scale`)

### Nginx Proxy (`proxy`)

- Acts as a reverse proxy in front of the Flask application
- Exposes port 80 to the host (mapped to port 8070)
- Routes incoming HTTP requests to the Flask service
- Can be used to distribute traffic across multiple Flask containers

---

## Docker Compose Responsibilities

Docker Compose is used to:

- Define and isolate services
- Create a shared network for inter-service communication
- Control which services are publicly exposed and which are internal
- Manage startup order using `depends_on`
- Provide a foundation for scaling and orchestration concepts

---

## What This Project Teaches

By building and running this setup, the following concepts are practiced:

- Structuring a multi-service application with Docker Compose
- Understanding the difference between internal and external service exposure
- Using Nginx as a reverse proxy for backend services
- Connecting application containers to Redis
- Recognizing the difference between Compose-based setups and Swarm-based deployments
- Understanding why `deploy.replicas` is Swarm-specific

---

## Scope and Limitations

This project is intentionally kept simple:

- No production-level security configuration
- Minimal error handling
- No persistence layer beyond Redis
- Intended for learning and experimentation only

---

## Purpose

This repository serves as a hands-on learning example for Docker Compose and service-based application design.  
It is meant as a reference project rather than a production-ready solution.
