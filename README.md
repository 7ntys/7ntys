# Julien Le Ber

Cloud & Infrastructure Engineer — Distributed Systems / Kubernetes

I build and study scalable infrastructure systems: autoscaling, observability and cloud-native workloads.

Currently focused on **GPU-aware autoscaling for AI workloads on Kubernetes**.

---

## What I work on

### GPU-Aware Autoscaler for Kubernetes

A custom autoscaling system written in Go that scales AI inference workloads using **real GPU usage and queue demand**, instead of CPU metrics.

Why it matters:
Traditional Kubernetes autoscaling (HPA) works well for web apps, but poorly for machine learning workloads.
AI inference is bursty, GPU-bound and latency-sensitive — scaling on CPU often reacts too late or wastes expensive GPUs.

My system:

* Reads GPU metrics (NVIDIA DCGM → Prometheus)
* Observes demand signals (Kafka consumer lag)
* Combines them with scaling policies (weighted scoring + hysteresis)
* Controls KEDA → HPA → pod replicas

Goal: scale **before** latency spikes and reduce idle GPU time.

Repository → [https://github.com/7ntys/gpu-autoscaler](https://github.com/7ntys/gpu-autoscaler)

---

## Areas of interest

* Kubernetes internals
* Autoscaling algorithms
* Distributed systems reliability
* Observability (Prometheus / Grafana)
* Cloud infrastructure architecture
* AI infrastructure (inference serving pipelines)

---

## Background

I’m an infrastructure-focused engineer with experience across cloud and on-prem environments.

I previously worked as a Cloud Engineer where I:

* built an internal AI assistant based on company cloud architecture standards
* automated infrastructure operations and certificate management
* handled production cloud requests and incident analysis

I’m currently working on research around autoscaling strategies for AI pipelines.

---

## Tech stack

Go · Kubernetes · KEDA · Docker · Terraform · Linux
Prometheus · Grafana · Kafka · Networking · CI/CD

Cloud: AWS · GCP · Azure

---

## Certifications

* AWS Certified Solutions Architect – Associate
* Microsoft Azure Administrator Associate
* Microsoft Azure Solutions Architect Expert
* Certified Kubernetes Administrator

---

## Contact

Paris, France
[julienlb49@gmail.com](mailto:julienlb49@gmail.com)
