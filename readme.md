# Docker Course – Learning Projects and Index

This repository serves as a central index and documentation space for the Udemy course:

"Lerne alles zum Thema Docker (Dockerfiles, Docker Compose, bis hin zum Deployment mit Swarm oder Kubernetes)"

Instructor: Jannis Seemann

The goal of this repository is to document the learning path, summarize core concepts, and collect hands-on projects created while following the course. It is intended as a long-term reference rather than a polished product repository.

---

## Course Scope

The course covers Docker from fundamental concepts to advanced deployment scenarios, including:

- Docker architecture and core concepts
- Building and managing Docker images
- Writing efficient Dockerfiles
- Multi-stage builds
- Docker Compose for multi-container applications
- Volumes and persistent data
- Networking concepts in Docker
- Container orchestration with Docker Swarm
- Introduction to Kubernetes
- Deployment and production best practices

---

## Repository Structure

The repository is organized by course sections. Each folder contains notes, examples, and small practice projects related to the respective topic.

---

## Table of Contents

### 01 – Introduction and Docker Basics

- What Docker is and what problems it solves
- Containers versus virtual machines
- Docker Engine and basic architecture
- Local installation and setup

Directory: `01_basics/`

---

### 02 – Docker Images

- Understanding Docker images and layers
- Image caching and versioning
- Building and running images
- Working with tags and registries

Directory: `02_images/`

---

### 03 – Dockerfiles

- Structure and syntax of Dockerfiles
- Core instructions (`FROM`, `RUN`, `COPY`, `CMD`, `ENTRYPOINT`)
- Best practices for maintainable Dockerfiles
- Multi-stage builds for optimized images

Directory: `03_dockerfiles/`

Practice project:

- Containerizing a simple application using a custom Dockerfile

---

### 04 – Container Lifecycle and Debugging

- Starting, stopping, and removing containers
- Inspecting running containers
- Viewing logs and debugging issues
- Resource limits and container constraints

Directory: `04_container_lifecycle/`

---

### 05 – Volumes and Persistent Data

- Difference between bind mounts and named volumes
- Persisting data across container restarts
- Managing and inspecting volumes

Directory: `05_volumes/`

Practice project:

- Running a database container with persistent storage

---

### 06 – Docker Networking

- Docker network drivers (bridge, host, overlay)
- Container-to-container communication
- Port exposure and basic security considerations

Directory: `06_networking/`

---

### 07 – Docker Compose

- Introduction to Docker Compose
- Defining services in `docker-compose.yml`
- Managing multi-container applications
- Service dependencies and environment configuration

Directory: `07_docker_compose/`

Practice project:

- Full-stack application using Docker Compose (frontend, backend, database)

---

### 08 – Docker Swarm

- Swarm architecture and core concepts
- Nodes, services, and stacks
- Scaling services and rolling updates

Directory: `08_docker_swarm/`

Practice project:

- Deploying a containerized application as a Swarm stack

---

### 09 – Kubernetes (Introduction)

- Motivation and high-level concepts
- Pods, deployments, and services
- Differences between Docker Swarm and Kubernetes
- First deployment examples

Directory: `09_kubernetes/`

---

### 10 – Deployment and Best Practices

- Production-ready Docker images
- Handling environment variables and secrets
- Basic security best practices
- Introduction to CI/CD concepts

Directory: `10_deployment_best_practices/`

---

## Learning Projects Overview

| Project                | Description                                | Stack          |
| ---------------------- | ------------------------------------------ | -------------- |
| Docker Basics Demo     | Basic container and image usage            | Docker         |
| Dockerfile Application | Containerized application using Dockerfile | Docker         |
| Compose Full Stack     | Multi-service application                  | Docker Compose |
| Swarm Deployment       | Orchestrated deployment                    | Docker Swarm   |
| Kubernetes Intro       | Initial Kubernetes deployment              | Kubernetes     |

---

## Purpose of This Repository

This repository is meant to:

- Document the learning process in a structured way
- Provide practical examples for later reference
- Serve as a personal knowledge base for Docker-related topics
- Support future production and deployment work

---

## Credits

Course:
"Lerne alles zum Thema Docker (Dockerfiles, Docker Compose, bis hin zum Deployment mit Swarm oder Kubernetes)"

Instructor:
Jannis Seemann

---

## License

This repository is intended for educational purposes only.  
All course materials remain the property of their respective owners.
