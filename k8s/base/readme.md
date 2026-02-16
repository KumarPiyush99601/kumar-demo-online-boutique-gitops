**Portfolio project demonstrating production-grade DevOps practices on Kubernetes**  
*(Local phase – full GitOps + cloud deployment coming soon)*

## Overview

This repository contains the **local Minikube deployment** of **Google's Online Boutique** — a cloud-native microservices demo application with **11 polyglot services** (Go, Python, Node.js, Java, C#).

The goal is to build and showcase a **complete, enterprise-ready DevOps platform**:

- End-to-end Kubernetes deployment
- GitOps with Argo CD (planned)
- Observability stack (Prometheus/Grafana/Loki/Tempo – planned)
- DevSecOps (Trivy, Kyverno – planned)
- Infrastructure as Code (Terraform for EKS/AKS – planned)

**This folder is the Minikube validation phase** — fully working app running on a single-node cluster for quick iteration and testing.

**Why this project?**  
To demonstrate senior-level DevOps skills focusing on Kubernetes, microservices, GitOps, and observability.

## Features (Current – Minikube Version)

- Deployed **11 microservices** from Google's official Online Boutique demo
- Exposed frontend via **LoadBalancer** service (simulated locally with `minikube tunnel`)
- Polyglot architecture: Go (frontend, payment, shipping), Python (recommendation), Node.js (currency), etc.
- Internal gRPC communication + Redis (cart) + in-memory datastores
- Verified full user flow: browse → add to cart → checkout → order confirmation

